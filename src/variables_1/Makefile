# print out every info about every .md file
print: $(wildcard *.md) hey
	ls -la $?
	echo $?

hey: one two
	echo $@ #target name

	echo $? #all dependencies newer than the target

	echo $^ #all dependencies

	echo $< #the first dependency

	touch hey

one:
	touch one

two:
	touch two

clean:

	rm -f hey one two
