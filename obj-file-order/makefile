.PHONY: common success failure

all: failure success

common:
	gcc -c first.c -o first.o 
	gcc -c last.c -o last.o
	gcc -c main.c -o main.o

failure: common
	gcc first.o last.o main.o -o fail.out

success: common
	gcc main.o last.o first.o -o success.out

