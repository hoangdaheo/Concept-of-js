# What is async?

- ans: async code is executed after a task that runs in the **background** finishes
- ans: not-blocking
- ans: execution doesn't wait for an async task to finish its work
- _need callback to implement async behavior_ => _but it's not mean callback automatically make code async_ (ex: array.map take callback but not async)

# What is sync?

- ans: executed line by line
- long-running operations block code

# What is thread of execution? --- **background**

- ans: part of execution context that actually executes the code in computer's CPU
- mk: that is a box cover all code, and stack by each instruction. (each line waits for previous line to finish)

# What is AJAX?

- ans: allow us to communicate with remote web servers in an async way.
- ans: can request data from web servers dynamically

# API

- ans: Piece of software can be used by another piece of software, in order to allow application to talk to each other.

# AJAX

- use to fetch data, and X means XML but this is old concept, nowadays we use JSON data format in request.

# TCP/IP

- TCP: transmission control protocol
- IP: internet protocol
- communication protocol that define how data travel across the web
- internet fundamental control system
- set the rules about how data moves on the internet.

1. break request to small chunk (it's called packet)
2. all packets arrive at their final destination, _TCP_ will reassemble all packets into the original req or res
3. _IP_ is send and route packets through the internet. (ensure they arrive at the destination they should go using IP address on its Packet)

# What is promise?

- ans: An obj that is used as a placeholder for the future result of an asynchronous operation.
- or: a container for an async delivered value ( or a container for a future value)

**EX**

1. when i bought a ticket that promise that i will receive money if i guess correct outcome
2. buy ticket (promise)
3. lottery draw happen _async_
4. if correct outcome, i receive money (cause it was promise)

## What is the diff between callback and promise?

- ans: no longer need to rely on events and callback passed into async to handle async results.
- ans: ev and cb sometime unpredictable results
- ans: chain promise for a sequence of async operations instead nesting callback.

## Anatomy of Promise (state in promise)

1. Pending (Before the future value is available) (doing...)
2. Setted (has finished)

- Fufilled (Success) : _the value is now available_
- Rejected () : _an error happened_

## Consume promise

- When we already have a promise. And using promise to display.
