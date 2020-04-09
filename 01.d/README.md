
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









# $(if $1, ...) -- If $1 is not empty, then...
# $(firstword $(l)) -- where l := apple orange -- would be apple (gets first word in list)
# $(call print_all,$(wordlist 2,$(words $1),$1))
#
# This is to call print_all with the list $1 without the first element, i.e., the tail of $1
# $(wordlist) lets you select a sublist (1-based)
# $(wordlist, start_index, length, list)
# 
# $(words $1) gives you the length of $1. 
# Index 2 - $(words $1) is in index beyond the end of the list, but Make ignores this.
# $1 - list of words to print
print_all = \
	$(if $1, \
			$(info $(firstword $1)) \
			$(call print_all,$(wordlist 2,$(words $1),$1)) \
		)
list := Hi there Nick, I hope this hint helps!
all:
	@: $(call print_all,$(list))
