CXX = icc
CXXFLAGS = -O0 -fopenmp

AR = /usr/bin/ar

MBPOL_OBJ = libmbpol.o \
            poly-2b-v6x.o poly-2b-v6x-nogrd.o \
            poly-3b-v2x.o poly-3b-v2x-nogrd.o \
            ttm4-es.o ttm4-smear.o gammq.o tang-toennies.o ps.o \
            x2b-dispersion.o x2b-v9x.o x3b-v2x.o mbpol.o

all: libmbpol.a

libmbpol.a: $(MBPOL_OBJ)
	$(AR) cru libmbpol.a $(MBPOL_OBJ)

clean:
	rm -f *.a *.o
