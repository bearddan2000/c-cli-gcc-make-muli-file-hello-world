# Makefile reads top to bottom

# 'main.o' forces make to do main.o task first
main: main.o
	gcc main.o greeting.o -o main

main.o: greeting.o
	gcc -c main.c -o main.o

# '-L' links the header file
greeting.o:
	gcc -c greeting.c -L ./greeting.h -o greeting.o
