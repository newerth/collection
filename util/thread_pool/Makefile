TARGET := tpool
SOURCES := $(wildcard *.c)
OBJECTS := $(SOURCES: .c=.o)

CC := gcc
CFLAGS := -ggdb
LIBS := -lpthread

%.o: %.c
	$(CC) $(CFLAGS) -c $< -o $@

all: $(OBJECTS)
	$(CC) $(CFLAGS) -o $(TARGET) $(OBJECTS) $(LIBS)

clean:
	rm -rf $(TARGET) core *.o

.PHONY:clean

