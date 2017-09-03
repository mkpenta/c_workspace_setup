#To use this make file, navigate to the directory containing the makefile and type "make"
#		

all: hello

hello: hello.c
	gcc -std=c11 -o hello hello.c
	
clean:
	rm hello

#In  a make file we need to specify how to build the program. We do this by creating targets and rules.
# the name to the left of the colon is the target. to the right are the prerequisite to make the target 
# the line follwing the target is the rule. this is tab indented and is the command to compile and make the program. 
# 
# !!--> It must be on TAB indented on level from the target. It cannot be spaces <--!!
# 
# when we specify make without any other information we mean make all. So make looks for the target all and findes it has
# a prerequisite condition, hello. To make all we need to make hello first. 
# 
# Make looks for the target hello and finds it has a prequisite of hello.c (which is ok as long as that file exists) and since this
# is not another target, it can build hello. The all rule can be built. 
# 
# The clean rule can be used to clean up previously built programs. to run the clean rule
# type: make clean
# 
# you can specify any rule when calling make. To build this program you could also type "make hello" 
# one make file can make many programs.

# the hello rule explained:
#   gcc is the compiler
#   -std=c11 forces the compiler to use the C11 standard 
#   -o is the output flag. It sets the name for the program output by the compiler.

# the clean rule explained:
#   rm is the remove command
#   hello is the file to remove
