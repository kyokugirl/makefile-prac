all: f1.o

foo: f1.o f2.o

f1.o f2.o :
	touch $@
	echo $@

clean:
	rm -f *.o
