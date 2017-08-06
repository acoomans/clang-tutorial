CPP = clang++
CPPFLAGS = -g -O3 -std=c++11 -I ~/src/compiler/llvm-project/llvm/include/ -I ~/src/compiler/build/include/
BUILD = compiler
OBJ = lexer.cpp parser.cpp driver.cpp
	

all: $(BUILD)
	
$(BUILD): $(OBJ)
	mkdir -p build
	$(CPP) $(CPPFLAGS) -o build/$@ $^
	
.PHONY: clean

clean:
	rm $(BUILD)