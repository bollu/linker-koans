.PHONY: run
run:
	gcc -c main.c -o main.o
	ar rs main.a main.o
	ld  -o success.out /usr/lib/x86_64-linux-gnu/Scrt1.o  /usr/lib/x86_64-linux-gnu/crti.o /usr/lib/gcc/x86_64-linux-gnu/11/crtbeginS.o -L/usr/lib/gcc/x86_64-linux-gnu/11 -L/usr/lib/x86_64-linux-gnu -L/lib/x86_64-linux-gnu -L/usr/lib/x86_64-linux-gnu -L/usr/lib/  main.a  -lc /usr/lib/gcc/x86_64-linux-gnu/11/crtendS.o --dynamic-linker=/lib64/ld-linux-x86-64.so.2

	./success.out
