### Makefile Syntax

```
target: dependencies
	command
```
- target: the name of the target file
- dependencies: the files that the target depends on. these files must exist before the target is run.
- command: the command to run.

### The Essence of Make

Make decides run target. if t is not exist, make will create it.
if the depencies changed since target was last compiled, make should recompile it.
to make this happen, make uses the filesystem timesatamps.

### Variables

Variables are used to store values that can be used in the makefile. It can only be strings.
Referece variables using either `${}`, `$()`

```
variables := file1, file2

target: $(variables)
  command

file1:
  command
file2:
  command
```
