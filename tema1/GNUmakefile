CLAGS = -Wall -g
all: build run clean
list.o:
	gcc -c utils/list.c -o list.o
hashmap.o:
	gcc -c utils/hashmap.c -o hashmap.o
command.o:
	gcc -c utils/command.c -o command.o
tema.o:
	gcc -c tema1.c -o tema.o
build:list.o hashmap.o command.o tema.o
	$(CC) $(CFLAGS) tema.o list.o hashmap.o command.o -o so-cpp
.SILENT:
run: 
	make clean
	./so-cpp -DNUMAR=1 -Iutils example.c -Ooutput.txt
	echo "----------------------------------------------------"
clean:
	rm -f *.o

	
