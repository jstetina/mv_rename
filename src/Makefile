CC = gcc
CFLAGS = -Wall -Wextra -Werror -std=c17 

SRC_FILES = $(wildcard $(SRC_DIR)/*.c)
EXECUTABLE = mv

all: $(EXECUTABLE)

$(EXECUTABLE): mv.o cli.o helper.o
	$(CC) $(CFLAGS) -o $@ $^

%.o: %.c
	$(CC) $(CFLAGS) -c $< -o $@

clean:
	rm -f *.o mv
