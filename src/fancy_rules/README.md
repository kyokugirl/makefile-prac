## Fancy Rules


### Implicit Rules
magic/automatic rules.

- `CC`: Program for compiling C programs; default cc
- `CXX`: Program for compiling C++ programs; default g++
- `CFLAGS`: Extra flags to give to the C compiler
- `CXXFLAGS`: Extra flags to give to the C++ compiler
- `CPPFLAGS`: Extra flags to give to the C preprocessor
- `LDFLAGS`: Extra flags to give to compilers when they are supposed to invoke the linker


### Static Pattern Rules
write less in a Makefile
```Makefile
targets... : target-pattern: dependencies-patters...
	commmands
```


### Static Pattern Rules and Filter
`filter` function can be used in Static rules to match the correct files.

+ `.PHONY`
Adding `.PHONY` to a target will prevent Make from confusing the phony target with a file name.
use for avoiding a conflict with a file or the same name or improving performance.
(https://www.gnu.org/software/make/manual/make.html#Phony-Targets)

### Pattern Rules
- A way to define your own implict rules
- A simpler form of static pattern rules

### Double-Colon Rules
allow multiple rules to be defined for the same target.
