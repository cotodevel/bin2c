BINNAME = bin2c
HEADERS = 
OBJECTS = $(BINNAME).o
VPATH :=	../src
all:	$(BINNAME)

%.o: %.c $(HEADERS)
	gcc -c $< -o $@

$(BINNAME): $(OBJECTS)
	gcc $(OBJECTS) -o $@
	-rm -f $(OBJECTS)

clean:
	-rm -f $(OBJECTS)
	-rm -f $(BINNAME)