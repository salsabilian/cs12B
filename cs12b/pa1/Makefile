#Shayan Salsabilian
#ssalsabi
#cs 12B
#1/16/2019
#creates the Search.class and creates the Search jar file
#Makefile
#------------------------------------------------------------------------------
# Another Makefile with macros
#------------------------------------------------------------------------------
JAVASRC    = Search.java 
SOURCES    = README Makefile $(JAVASRC)
MAINCLASS  = Search
CLASSES    = Search.class
JARFILE    = Search
SUBMIT     = submit cmps012b-pt.w19 pa1 

all: $(JARFILE)

$(JARFILE): $(CLASSES)
	echo Main-class: $(MAINCLASS) > Manifest
	jar cvfm $(JARFILE) Manifest $(CLASSES)
	rm Manifest
	chmod +x $(JARFILE)

$(CLASSES): $(JAVASRC)
	javac -Xlint $(JAVASRC)

clean:
	rm $(CLASSES) $(JARFILE)

submit: $(SOURCES)
	$(SUBMIT) $(SOURCES)

check:
	ls  /afs/cats.ucsc.edu/class/cmps012b-pt.w19/pa1/ssalsabi
