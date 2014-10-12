#Makefile
CC=g++ 
LIB=-lglut -lGLU -lGL
INCDIR=-I../
ALIB=../matplotpp.a

CMD=$(CC) $(LIB) $(INCDIR)

CC_FILES = $(wildcard *.cc)
BINS = $(patsubst %.cc, %, $(CC_FILES))
BINSI = $(patsubst %.cc, $(GOBIN)/%, $(CC_FILES))

build: ${BINS}

install: ${BINSI}

${GOBIN}:
	mkdir -p $@

%: %.cc
	$(CMD) -o $@ $< $(ALIB)

${GOBIN}/%: % ${GOBIN}
	cp $< ${GOBIN}

clean:
	rm -f ${BINS}
