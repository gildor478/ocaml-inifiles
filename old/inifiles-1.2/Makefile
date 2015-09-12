-include Makefile.conf

SOURCES=parseini.mly inilexer.mll inifiles.mli inifiles.ml
RESULT=inifiles
PACKS=pcre

LIBINSTALL_FILES=$(wildcard *.mli *.cmi *.cma *.cmxa *.a *.so)
OCAMLDOCFLAGS=-colorize-code

all: debug-code-library
opt: native-code-library
reallyall: byte-code-library native-code-library
install: libinstall
uninstall: libuninstall

-include OCamlMakefile
