
## Stack and queue
![](https://pimages.toolbox.com/wp-content/uploads/2023/05/19105134/image-58-1024x258.png)

## stack
![](https://media.geeksforgeeks.org/wp-content/cdn-uploads/20221219100314/stack.drawio2.png)

A stack follows the Last In First Out (LIFO) order, meaning the element that is inserted last will be the first one to be removed. It has only one end called the top, where both insertion (push) and deletion (pop) operations take place. Checking if the stack is empty is done by comparing the top pointer with -1, indicating no element in the stack. Similarly, checking if the stack is full is done by comparing the top pointer with the maximum size of the stack.
## queue
![](https://media.geeksforgeeks.org/wp-content/uploads/FIFO.jpg)

On the other hand, a queue follows the First In First Out (FIFO) order, where the element that is inserted first will be the first one to be removed. It has two ends, known as the rear and front, used for insertion (enqueue) and deletion (dequeue) operations, respectively. Checking if the queue is empty is typically done by comparing the front pointer with -1. The condition for a full queue is often defined by comparing the rear pointer with the maximum size of the queue.

## Additional information
![](https://miro.medium.com/v2/resize:fit:1400/format:webp/1*zKnDkJpL-4GQ36kzrDiODQ.png)

While stacks have a simple implementation without the need for additional pointers, queues involve two pointers (front and rear) for efficient insertion and deletion. Additionally, queues have various types, such as circular queues (where the rear and front wrap-around), double-ended queues (allowing insertion and deletion at both ends), and priority queues (where elements are assigned priorities).

