obj = asscat.o
bin = asscat
root = ../..
lib_so = $(root)/libassfile.so.0.1

CFLAGS = -pedantic -Wall -g -I$(root)/src
LDFLAGS = -L$(root) -Wl,-rpath,$(root) -lassfile

$(bin): $(obj) $(lib_so)
	$(CC) -o $@ $(obj) $(LDFLAGS)

.PHONY: clean
clean:
	rm -f $(obj) $(bin)
