CC=g++ 
LIBS=-lGL -lGLU -lglfw -lGLEW
INC=-I../../../common
CFLAGS=-std=c++11 -g

buildAll: main.out shader.o

shader.o: ../../../common/shader.cpp
	$(CC) $(CFLAGS) $^ -c  $(LIBS) $(INC)

main.out: main.cpp shader.o
	$(CC) $(CFLAGS) $^ -o  $@ $(LIBS) $(INC)

.PHONY: clean
clean:
	rm *.out
