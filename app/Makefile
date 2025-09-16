CXX = g++
CXXFLAGS = -g3 -Wall -Wextra -Wpedantic -std=c++17
MKDIR = mkdir -p

LIBS = -lm

directorios:
	$(MKDIR) build dist

build/main.o: directorios main.cpp
	$(CXX) $(CXXFLAGS) -c main.cpp -o build/main.o

all: clean build/main.o
	$(CXX) $(CXXFLAGS) -o dist/programa \
	build/main.o \
	$(LIBS)
	rm -fr build

clean:
	rm -fr *.o a.out core programa dist build

.DEFAULT_GOAL := all
