CC = /usr/local/bin/gcc-5
TARGET = outO2g

all: main.o predator.o map_function.o data_struct.o select_lib.o
	$(CC) -O2 -o $(TARGET) main.o predator.o \
							map_function.o data_struct.o \
							 select_lib.o
	open $(TARGET)

%.o: %.c types.h
	$(CC) -O2 -c $<

clean:
	rm *.o