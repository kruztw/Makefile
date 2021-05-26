# @<cmd> : silence
# -<cmd> : Don't stop even error occured
# $@ : target
# $< : first prerequisite
# $^ : all prerequisite
# $(wildcard *.c) : *.c in this dir

# 第ㄧ順位: 賦值 (a=1) , := , ?=
# 第二順位: 展開 (b=$a)

a  = 1          # a = 1
a ?= 2          # a = 1  (if not define a then a = 2)
b  = $a         # b = 3
c := $a         # c = 1
a  = 3          # a = 3

all: arg1 arg2
	@echo $a $b $c
	@-rm fo
	@echo $@
	@echo $<
	@echo $^
	@echo $(wildcard *.c)


