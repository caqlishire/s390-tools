include ../common.mak

lib = libdasd.a

all: $(lib)

objects = dasd_sys.o dasd_ioctl.o

$(lib): $(objects) Makefile

install: all

clean:
	rm -f *.o $(lib)
