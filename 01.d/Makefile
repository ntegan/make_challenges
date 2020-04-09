# 2020_04_09 word capitalizer
# 		Pete's Challenge
#
#http://patorjk.com/software/taag/#p=display&f=Big&t=Version%202
# https://www.gnu.org/software/make/manual/make.html

print2 = \
				 $(if $1, \
				 		$(if $2, \
							$(call print2,$(wordlist 2,$(words $1),$1),$(wordlist 2,$(words $2),$2),$(subst $(firstword $1),$(firstword $2),$(3))) \
						),$(info $3))

#lowercase list
ll := a b c d e f g h i j k l m n o p q r s t u v w x y z
#uppercaselist
ul := A B C D E F G H I J K L M N O P Q R S T U V W X Y Z

%:
	@: $(call print2,$(ll),$(ul),$*)
