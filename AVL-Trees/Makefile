CC := gcc
CFLAGS = -g -Wall -Werror -std=c11

SOURCES = BST.c treeLab.c

OUTPUT = treeLab 

all: $(OUTPUT)

%.o: %.c BST.h
	$(CC) $(CFLAGS) -c $< -o $@

$(OUTPUT): $(SOURCES:.c=.o)
	$(CC) $(CFLAGS) $^ -o $(OUTPUT)

clean:
	rm -f *.o $(OUTPUT)
