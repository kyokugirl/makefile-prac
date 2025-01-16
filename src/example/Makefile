x := blah

blah: blah.o
	cc blah.o -o blah #runs third
	touch $x #change the timestamp to newer

blah.o: blah.c
	cc -c blah.c -o blah.o #runs second

blah.c:
	echo "int main() { return 0; }" > blah.c #runs first

clean:
	rm -f  blah blah.o blah.c
