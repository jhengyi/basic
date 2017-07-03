CFLAGS=-fPIC

SOURCE_OBJS= sample.o

DYNANIC_LIB=libsample.so
STATIC_LIB=libsample.a

all:$(DYNANIC_LIB) $(STATIC_LIB)

$(STATIC_LIB) : $(SOURCE_OBJS)
		$(AR) rcs $@ $^ 
		#cp -f $@ ../../lib/

$(DYNANIC_LIB): $(SOURCE_OBJS)
		$(CC) -shared $(CFLAGS) -o $@ $^
		#cp -f $@ ../../../lib/

clean:
		rm -rf *.o $(DYNANIC_LIB) $(IPCAMSOCKET_OBJS) 

