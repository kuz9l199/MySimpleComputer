all : MSC

MSC : program.o smc.a
	gcc -o MSC program.o -L. msc.a

program.o : program.c
	gcc -c program.c

msc.a : MemoryFunc.o CommandFunc.o RegistFunc.o
	ar cr msc.a MemoryFunc.o CommandFunc.o RegistrFunc.o

MemoryFunc.o : Memory.c
	gcc -c MemoryFunc.c

CommandFunc.o : CommandFunc.c
	gcc -c Command.c

RegistrFunc.o : RegistrFunc.c
	gcc -c RegistrFunc.c

clear :
	rm * .o
	rm * .exe
	rm * .a
	
