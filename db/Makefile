CC=g++
CFLAGS=-std=c++17 -c -g -O3 -Wall -fgnu-tm -D SPLINTERDB_PLATFORM_DIR=platform_linux
INCLUDES=-I ../
SOURCES=$(wildcard *.cc)
OBJECTS=$(SOURCES:.cc=.o)

all: $(SOURCES) $(OBJECTS)

.cc.o:
	$(CC) $(CFLAGS) $(INCLUDES) $< -o $@

clean:
	$(RM) $(OBJECTS)

