.PHONY: common success failure

all: success failure

common:
	gcc -c first.c -o first.o 
	ar rs first.a first.o
	gcc -c last.c -o last.o
	ar rs last.a last.o
	gcc -c main.c -o main.o
	ar rs main.a main.o

failure: common
	-gcc first.a last.a main.a -o fail.out
	@echo "^^FAILURE!^^"

# Linking static libs should be given starting from main(), walking upwards.
success: common
	gcc main.a last.a first.a -o success.out -v
	./success.out
	@echo "^^SUCCESS!^^"

