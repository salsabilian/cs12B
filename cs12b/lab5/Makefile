#------------------------------------------------------------------------------
# Shayan Salsabilian
# ssalsabi
# 2/19/19
# 12B
# Makefile for any ADT and its test client
# Makefile
#------------------------------------------------------------------------------

ADT_NAME  = Dictionary
SOURCES   = $(ADT_NAME).c $(ADT_NAME)Client.c
OBJECTS   = $(ADT_NAME).o $(ADT_NAME)Client.o
HEADERS   = $(ADT_NAME).h
EXEBIN    = $(ADT_NAME)Client
FLAGS     = -std=c99 -Wall
all: $(EXEBIN)

$(EXEBIN) : $(OBJECTS) $(HEADERS)
	gcc -o $(EXEBIN) $(OBJECTS)

$(OBJECTS) : $(SOURCES) $(HEADERS)
	gcc -c $(FLAGS) $(SOURCES)

clean :
	rm -f $(EXEBIN) $(OBJECTS)
submit:
	submit  cmps012b-pt.w19 lab5 README Makefile Dictionary.c DictionaryTest.c Dictionary.h DictionaryClient.c

check:
	valgrind --leak-check=full $(EXEBIN)
check2:
	ls  /afs/cats.ucsc.edu/class/cmps012b-pt.w19/lab5/ssalsabi 
