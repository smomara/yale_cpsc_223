CC=gcc
CFLAGS=-g3 -Wall

# extra flags for treeTest
TREETEST_CFLAGS=-DDEBUG_SPLAY -DTEST_MAIN

all:

test: treeTest
	valgrind -q ./treeTest

treeTest: tree.c tree.h
	$(CC) $(CFLAGS) $(TREETEST_CFLAGS) -o $@ $<

speedTest: speedTest.o tree.o
	$(CC) $(CFLAGS) -o $@ $^

clean:
	$(RM) *.o treeTest speedTest
