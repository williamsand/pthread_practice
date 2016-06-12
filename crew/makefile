CC= gcc
#SRCS = $(./src/ wildcard *.c)
#OBJS = $(SRCS:%.c=%.o)
OBJS += crew.o

INCLUDE += ../include 

CFLAGS += -I $(INCLUDE)
CFLAGS += -lpthread
CFLAGS += -lrt

all:crew

crew:$(OBJS)
	$(CC) $^ -o $@ $(CFLAGS)
	
$(OBJS):%.o:%.c
	$(CC) -c $^ -o $@ $(CFLAGS) 

clean:
	rm -rf *.crew
	
