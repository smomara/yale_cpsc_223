CC=gcc
CFLAGS=-g3 -Wall

all: test_radixSort sortInput

test: all
	./test_radixSort

test_radixSort: test_radixSort.o radixSort.o
	$(CC) $(CFLAGS) -o $@ $^

sortInput: sortInput.o radixSort.o
	$(CC) $(CFLAGS) -o $@ $^

clean:
	$(RM) test_radixSort sortInput *.o
