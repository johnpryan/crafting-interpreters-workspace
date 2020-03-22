JCC = javac
JFLAGS = -g
BUILD_DIR=$(PWD)/src/com/craftinginterpreters/lox

src = $(wildcard *.java)
clss = $(wildcard *.class)

default: all

test: $(src)
	$(JCC) $(JFLAGS)

all: $(BUILD_DIR)/Lox.java $(BUILD_DIR)/Scanner.java $(BUILD_DIR)/Token.java $(BUILD_DIR)/TokenType.java
	$(JCC) $(JFLAGS) $(BUILD_DIR)/Lox.java $(BUILD_DIR)/Scanner.java $(BUILD_DIR)/Token.java $(BUILD_DIR)/TokenType.java

clean:
	$(RM) $(BUILD_DIR)/*.class
