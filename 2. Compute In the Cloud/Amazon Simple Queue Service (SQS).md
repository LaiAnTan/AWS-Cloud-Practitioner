#service #module_2

**Message queueing service** that is able to **send, store and receive messages between software components**.

Messages are sent into a **queue**, retrieved from the queue, processed and then deleted.

This prevents messages from being dropped after a certain amount of time, as they would always stay in the queue until they are handled.

This approach enables the separate application components to work more efficiently and independently.