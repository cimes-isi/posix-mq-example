# POSIX Message Queue Example

A simple producer/consumer example using POSIX Message Queues.

## Building

Build out-of-source using CMake:

``` sh
mkdir BUILD
cd BUILD
cmake ..
make
```

## Usage

To run, start a producer:

``` sh
./posix-mq-example 0
```

then start a consumer:

``` sh
./posix-mq-example 1
```

The producer sends a predefined number of messages to the consumer, then both terminate.
