CC := g++
CFLAGS := -Wall -g
BIN := bin
TARGET := $(BIN)/lesson02

SRCS := $(wildcard *.cpp)
OBJS := $(patsubst %.cpp,%.o,$(SRCS))


all: bin $(TARGET)

$(TARGET): $(OBJS)
	$(CC) -o $@ $^

bin:
	mkdir $(BIN)

%.o: %.cpp
	$(CC) $(CFLAGS) -c $<

clean:
	rm -rf $(BIN)
	rm -rf *.o
	rm -rf $(TARGET)

.PHONY: all clean
