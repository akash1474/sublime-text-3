# The location where SFML is installed
SFML_DIR=D:/Others/SFML-2.5.1

# Location where SFML libraries are located
LIBDIR=$(SFML_DIR)/lib

# Arguments to pass to the compiler
CFLAGS=-I $(SFML_DIR)/include

# SFML (and other) libraries that need to be linked with
LIBS=-lsfml-graphics -lsfml-window -lsfml-system

# Set the rule that links the executable as the default
# This is the default because it is *first* in the file,
# not because of it's name!
default: sfml
	LD_LIBRARY_PATH=$(LIBDIR) ./sfml

# Create the executable file
sfml: main.o
	g++ -o sfml -L $(LIBDIR) $(LIBS) main.o

# Compile the source file
main.o: main.cpp
	g++ -c main.cpp $(CFLAGS) -o main.o

# For running
run: sfml
	LD_LIBRARY_PATH=$(LIBDIR) ./sfml