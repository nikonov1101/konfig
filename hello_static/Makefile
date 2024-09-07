# /usr/bin/cc

CC := musl-gcc -g3 -Wall -Wextra -Wconversion -Wdouble-promotion -Wno-unused-parameter -Wno-unused-function -Wno-sign-conversion -fsanitize=undefined -static

all: clean hello_world

hello_world: hello_world.o
	$(CC) -o $@ $<

hello_world.o: hello_world.c
	$(CC) -c -o $@ $<

clean:
	rm -f hello_world hello_world.o
