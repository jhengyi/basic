#ROOT_DIR:/home/willie/Blowfish_text
#include ./Makefile.parm

MY_OBJS = test.o

CFLAGS =-I../.

LIBS =-L../ -lsample

default:all
all: my_test

my_test: $(MY_OBJS)
	#$(CC) $(CFLAGS) -o $@ $^ $(LIBS) $(LDFLAGS) 

	$(CC) $(CFLAGS) -static -o $@ $^ $(LIBS) 
clean:
	@rm -vrf *.o my_test $(MY_OBJS)




