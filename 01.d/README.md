
In Make, I want a function that can capitalize all letters in a word, grasshopper (edited) 





2:04
I have an implementation of this already



this behavior:
~$ make foobar
FOOBAR





2:11
I will give you some hints
2:12
Examine these docs carefully https://www.gnu.org/software/make/manual/make.html#Functions
Do this to make Make not print out x is up to date.
all:
    @:$(info Hello, world!)
(edited)
gnu.orggnu.org
GNU make
GNU make
2:12
@:  is a weird construct I happened across
2:13
not in the documentation













very good
2:57
part 2

now do it with only one call to subst (by that I mean it only appears once in the Makefile )
2:57
one callsite


i.e., do it with an iterative process
