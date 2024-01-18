CC=g++
CFLAGS=-g -Wall
OBJ=obj
SRC=src
INC=include
BIN=bin
MAIN=main
EXE=main
OBJS=$(OBJ)/$(MAIN).o

all: $(BIN)/$(EXE)

run: all
	$(BIN)/$(EXE)

$(OBJ)/%.o: $(SRC)/main.cpp
	$(CC) $(CFLAGS) -o $@ -c $^

$(BIN)/$(EXE): $(OBJS)
	$(CC) $(CFLAGS) -o $@ $^

clean:
	rm -rf obj/* bin/*
