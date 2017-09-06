# Client/Server

A client server architecture using multi-threaded sockets implemented in C. User is able to ping websites and get minimum, maximum, and average request times. They can also check if their requests has been processed yet or what other users have requested.  

## Getting Started

### Prerequisites

Download server.c and client.c

### Compile and run instructions

Navigate to where you stored the files

1. Compile server.c
```
gcc -lpthread -lrt -o server server.c
```
2. Run server.c
```
./server
```

3. Compile client.c
```
gcc -o client client.c
```
4. Run client.c
```
./client <server computer name>   
eg: ./client linux60808
```

### Running commands

These are the available commands:

#### pingSites <argv[0]>, <argv[1]>, ... 
  Pings the given websites and displays their minimum, maximum, and average response times and the user's handle number. Each <argv[]> can be filled with a website     URL. Number of websites able to be pinged at once is limited by the character array size(1024).
  ```
  pingSites www.google.com, www.bing.com, www.cnn.com
  ```
  
#### showHandles 
  Shows all the handle numbers the server currently has received. 

#### showHandleStatus \<handle>
  Shows a specify handle's request and whether the request is in queue, in progress, or complete. 

#### showHandleStatus 
  Shows all the handles requests and whether they are in queue, in progress, or complete.

#### exit 
  Closes application.

#### help
  Shows all available commands and their syntax.



