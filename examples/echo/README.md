# Echo

This is a very basic echo client server example, the server accepts a single client at a time and echoes all
messages it receives.

Here is how to compile it with gcc:

`gcc -DNBN_GAME_CLIENT client.c shared.c -o client`

`gcc -DNBN_GAME_SERVER server.c shared.c -o server`

To run the server simply do:

`./server`

and to run the client:

`./client "some message"`

The client will run indefinitely and send the given string to the server every tick (30 times per second).