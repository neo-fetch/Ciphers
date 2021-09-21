   
CC = gcc
CFLAGS = -g -Wall
EXECUTABLE= cipher

all: cipher
cipher: vigenerecypher.c
	$(CC) $(CFLAGS) vigenerecypher.c -o $(EXECUTABLE)

clean:
	rm -rf *.o *.out *.gch $(EXECUTABLE)
leaks:
	valgrind --leak-check=yes --track-origins=yes -s ./$(EXECUTABLE)