SOURCE = hello.c
BIN = hello.exe
TXT = output.txts
CC = gcc
CFLAGS = -std=c18

$(BIN): $(SOURCE)
	$(CC) $(SOURCE) -o $(BIN) $(CFLAGS)

run: $(BIN)
	./$(BIN)

create_txt: $(BIN)
	./$(BIN) > $(TXT)

clean:
	rm -f $(BIN) $(TXT)