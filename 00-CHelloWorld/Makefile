SOURCE = hello.c
BIN = hello.exe
TXT = output.txt
CC = gcc
CFLAGS = -std=c18

$(BIN): $(SOURCE)
	$(CC) $(SOURCE) -o $(BIN) $(CFLAGS)

run: $(BIN)
	./$(BIN)

txt: $(BIN)
	./$(BIN) > $(TXT)

clean:
	rm -f $(BIN) $(TXT)