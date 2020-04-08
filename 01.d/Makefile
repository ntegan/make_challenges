# 2020_04_08 word capitalizer
# 		Pete's Challenge
#
#http://patorjk.com/software/taag/#p=display&f=Big&t=Version%202


# 
#
#  __  __       _       
# |  \/  |     (_)      
# | \  / | __ _ _ _ __  
# | |\/| |/ _` | | '_ \ 
# | |  | | (_| | | | | |
# |_|  |_|\__,_|_|_| |_|

%:
	@:$(call capitalize3,$*)





# __      __           _               ____
# \ \    / /          (_)             |___ \
#  \ \  / /__ _ __ ___ _  ___  _ __     __) |
#   \ \/ / _ \ '__/ __| |/ _ \| '_ \   |__ <
#    \  /  __/ |  \__ \ | (_) | | | |  ___) |
#     \/ \___|_|  |___/_|\___/|_| |_| |____/

capitalize3 =	 $(info \
							 		$(strip			 \
						 			$(subst a,A, \
									$(subst b,B, \
									$(subst c,C, \
									$(subst d,D, \
									$(subst e,E, \
									$(subst f,F, \
									$(subst g,G, \
									$(subst h,H, \
									$(subst i,I, \
									$(subst j,J, \
									$(subst k,K, \
									$(subst l,L, \
									$(subst m,M, \
									$(subst n,N, \
									$(subst o,O, \
									$(subst p,P, \
									$(subst q,Q, \
									$(subst r,R, \
									$(subst s,S, \
									$(subst t,T, \
									$(subst u,U, \
									$(subst v,V, \
									$(subst w,W, \
									$(subst x,X, \
									$(subst y,Y, \
									$(subst z,Z,$(1)))))))))))))))))))))))))))) \
								)


















# __      __           _               ___  
# \ \    / /          (_)             |__ \ 
#  \ \  / /__ _ __ ___ _  ___  _ __      ) |
#   \ \/ / _ \ '__/ __| |/ _ \| '_ \    / / 
#    \  /  __/ |  \__ \ | (_) | | | |  / /_ 
#     \/ \___|_|  |___/_|\___/|_| |_| |____|
#

capitalize2 =	 $(info \
							 			$(patsubst %a%,%A%,$(1)) \
							 			$(patsubst a%,A%,$(1)) \
							 			$(patsubst %a,%A,$(1)) \
									)


















# __      __           _               __ 
# \ \    / /          (_)             /_ |
#  \ \  / /__ _ __ ___ _  ___  _ __    | |
#   \ \/ / _ \ '__/ __| |/ _ \| '_ \   | |
#    \  /  __/ |  \__ \ | (_) | | | |  | |
#     \/ \___|_|  |___/_|\___/|_| |_|  |_|

#for i in `seq 65 $((64+26))`; do letter="$(printf "\x$(printf %x $i)")"; letter2="$(printf "\x$(printf %x $((i+32)))")"; echo '$(subst '"$letter2,$letter,"'$(1))'; done

#%:
#	@echo $* | tr '[:lower:]' '[:upper:]'
#

capitalize =	 $(info \
						 			$(subst a,A,$(1)) \
									$(subst b,B,$(1)) \
									$(subst c,C,$(1)) \
									$(subst d,D,$(1)) \
									$(subst e,E,$(1)) \
									$(subst f,F,$(1)) \
									$(subst g,G,$(1)) \
									$(subst h,H,$(1)) \
									$(subst i,I,$(1)) \
									$(subst j,J,$(1)) \
									$(subst k,K,$(1)) \
									$(subst l,L,$(1)) \
									$(subst m,M,$(1)) \
									$(subst n,N,$(1)) \
									$(subst o,O,$(1)) \
									$(subst p,P,$(1)) \
									$(subst q,Q,$(1)) \
									$(subst r,R,$(1)) \
									$(subst s,S,$(1)) \
									$(subst t,T,$(1)) \
									$(subst u,U,$(1)) \
									$(subst v,V,$(1)) \
									$(subst w,W,$(1)) \
									$(subst x,X,$(1)) \
									$(subst y,Y,$(1)) \
									$(subst z,Z,$(1)) \
								)


