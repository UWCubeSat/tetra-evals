CS := $(wildcard *.c)
OUTS := $(patsubst %.c, %, $(CS))

CFLAGS := $(CFLAGS) -O3 --lto
LDFLAGS := $(LDFLAGS) -lm

all: $(OUTS)

%: %.c
	$(CC) $(CFLAGS) -o $@ $< $(LDFLAGS)

clean:
	rm -f $(OUTS)

.PHONY: all clean
