.PHONY: all debug release clean

RELEASE_FLAGS = -O2 -Wall -DNDEBUG
DEBUG_FLAGS   = -g -O0 -Wall
RELEASE_EXEC  = kazino
DEBUG_EXEC    = kazino-dbg
SOURCE        = Kazino-Royal.cpp

all: debug release

debug: $(DEBUG_EXEC)

$(DEBUG_EXEC): Kazino-Royal.cpp
	g++ $(DEBUG_FLAGS) Kazino-Royal.cpp -o 

release: $(RELEASE_EXEC)

$(RELEASE_EXEC): Kazino-Royal.cpp
	g++ $(RELEASE_FLAGS) Kazino-Royal.cpp -o 

clean:
	rm -f $(RELEASE_EXEC) $(DEBUG_EXEC)
