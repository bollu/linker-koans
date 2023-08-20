.PHONY: flag noflag


all: noflag flag

flag:
	g++ a.c -o a.o -shared -Wl,-no-undefined -v

noflag:
	g++ a.c -o a.o -shared -v

