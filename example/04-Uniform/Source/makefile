CC=g++ 
LIBS=-lGL -lGLU -lglfw -lGLEW
CFLAGS=-std=c++11 -g

buildAll: main.out 

main.out: main.cpp
	$(CC) $(CFLAGS) $^ -o  $@ $(LIBS) $(INC)

.PHONY: clean
clean:
	rm *.out
