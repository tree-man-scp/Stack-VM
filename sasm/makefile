CFLAGS=-std=c++11

all: sasm

sasm: sasm.o lexer.o
	$(CXX) $(CFLAGS) sasm.o lexer.o -o $@

lexer.o: lexer.h lexer.cpp
	$(CXX) $(FLAGS) -c lexer.cpp

sasm.0: lexer.h sams.cpp
	$(CXX) $(FLAGS) -c sams.cpp

clean:
	rm -f sasm *.0 *.bin
