ALLFILES = rsync-and-debian.ps rsync-and-debian.html
all: $(ALLFILES)

clean:
	rm -f $(ALLFILES)

%.html: %.sgml
	linuxdoc -B html -s 0 $<

%.ps: %.sgml
	linuxdoc -B latex -o ps -p a4 $<

