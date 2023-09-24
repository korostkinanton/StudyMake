# Усложненный make-file.  Введены переменные для параметров компиляции и исполняемых файлов

.PHONY: all debug release clean

RELEASE_FLAGS = -O2 -Wall -DNDEBUG
DEBUG_FLAGS   = -g -O0 -Wall
RELEASE_EXEC  = hello
DEBUG_EXEC    = hello-dbg
#SOURCE        =

all: debug release

debug: hello-dbg

hello-dbg: hello.cpp
	g++ -g -O0 hello.cpp -o -Wall

release: hello

hello: hello.cpp
	g++ -O2 hello.cpp -o -Wall -DNDEBUG

clean:
	rm -f hello hello-dbg

