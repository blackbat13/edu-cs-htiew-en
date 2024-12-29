# Queue

## [:link: Problem description](../../../../algorithms/structures/queue.md)

## Implementation

```c linenums="1"
#include <stdio.h>
#include <stdlib.h>


typedef struct element {
    int value;
    struct element *next;
} element;

typedef struct Queue {
    element *front_el;
    int el_count;
} Queue;

void init(Queue *queue) {
    queue->front_el = NULL;
    queue->el_count = 0;
}

void push(int value, Queue *queue) {
    element *new_el = malloc(sizeof(element));

    new_el->value = value;
    new_el->next = NULL;

    if (queue->front_el == NULL) {
        queue->front_el = new_el;
        queue->el_count++;
        return;
    }

    element *last_el = queue->front_el;
    while (last_el->next != NULL) {
        last_el = last_el->next;
    }

    last_el->next = new_el;
    queue->el_count++;
}

int front(Queue *queue) {
    if (queue->front_el != NULL) {
        return queue->front_el->value;
    }
}

void pop(Queue *queue) {
    if (queue->front_el != NULL) {
        element *tmp = queue->front_el->next;
        free(queue->front_el);
        queue->front_el = tmp;
        queue->el_count--;
        return;
    }
}

void clear(Queue *queue) {
    element *tmp;
    while (queue->front_el != NULL) {
        tmp = queue->front_el->next;
        free(queue->front_el);
        queue->front_el = tmp;
    }
}

int is_empty(Queue *queue) {
    return queue->front_el == NULL;
}

int count(Queue *queue) {
    return queue->el_count;
}

int main() {
    int array[10] = {7, 3, 0, 1, 5, 2, 5, 19, 10, 5};
    Queue queue;

    init(&queue);

    for (int i = 0; i < 10; i++) {
        push(array[i], &queue);
    }

    printf("%d\n", count(&queue));

    while (!is_empty(&queue)) {
        printf("%d ", front(&queue));
        pop(&queue);
    }

    printf("\n");

    clear(&queue);

    return 0;
}
```

This code provides a simple implementation of a queue with basic operations such as initialization, pushing, popping, checking if empty, counting elements, and clearing the queue. Below is a short breakdown of the key components and functions.

### Structures

1. **element**: Represents a node in the linked list.

2. **Queue**: Represents the queue itself, containing a pointer to the front element and a count of elements.

### Functions

1. **init**: Initializes the queue by setting the front element to `NULL` and the element count to 0.

2. **push**: Adds a new element with the given value to the end of the queue.

3. **front**: Returns the value of the front element in the queue.

4. **pop**: Removes the front element from the queue.

5. **clear**: Empties the queue by freeing all elements.

6. **is_empty**: Checks if the queue is empty.

7. **count**: Returns the number of elements in the queue.

### Main Function

The `main` function demonstrates the usage of the queue:

1. Initializes a queue.
2. Pushes elements from an array into the queue.
3. Prints the count of elements in the queue.
4. Iterates through the queue, printing and popping each element.
5. Clears the queue.
