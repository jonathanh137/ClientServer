Compile and run instructions:

For server.c: 
gcc -lpthread -lrt -o server server.c
./server

For client.c:
gcc -o client client.c
./client <server computer name>   //eg: ./client linux60808
