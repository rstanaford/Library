CC=cc
CFLAGS=-Wall -g -std=gnu99

LIBS=
MYLIBS=

INCDIR=../inc
OBJDIR=../obj
BINDIR=../bin
TARGET= <##########>


_DEPS =
DEPS = $(patsubst %,$(INCDIR)/%,$(_DEPS)) 


_OBJS = <##########>
OBJS = $(patsubst %,$(OBJDIR)/%,$(_OBJS))






$(OBJDIR)/%.o: %.c $(DEPS)
	$(CC) -c -o $@ $< $(CFLAGS)

build: $(OBJS)
	$(CC) $(CFLAGS) -o $(BINDIR)/$(TARGET) $^ $(LIBS) $(MYLIBS)



.PHONY: clean

clean:
	rm -f $(BINDIR)/$(TARGET) $(OBJDIR)/*



