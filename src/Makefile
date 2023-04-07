# the compiler: gcc for C program
CC = gcc

#compiler flags:
#	-g		adds debugging information to the executable file
#	-Wall	turns on almost all compiler warnings
CFLAGS = -g -Wall

# Typing 'make' in the terminal will invoke this call to gol
all: lab6

# Creates an executable file for lab6 using:
# 	- memory_mgmt.o
lab6: memory_mgmt.o
	$(CC) $(CFLAGS) -o lab6 memory_mgmt.o 

# Creates an object file for memory_mgmt.o using:
#	- memory_mgmt.c
memory_mgmt.o: memory_mgmt.c
	$(CC) $(CFLAGS) -c memory_mgmt.c

# Typing 'make clean' will invoke a call to this section.
# 'gol' removes the executable file.
# '-.o' removes old object files.
# '*~' removes backup files.
clean:
	$(RM) gol *.o *~