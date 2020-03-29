JCC = javac
JFLAGS = -g
BUILD_DIR=$(PWD)/src/com/craftinginterpreters/lox
TOOL_DIR=$(PWD)/src/com/craftinginterpreters/tool

src = $(wildcard *.java)
clss = $(wildcard *.class)

default: all

generate: $(TOOL_DIR)/GenerateAst.java
	$(JCC) $(JFLAGS) $(TOOL_DIR)/GenerateAst.java

all: generate $(BUILD_DIR)/Lox.java $(BUILD_DIR)/Scanner.java $(BUILD_DIR)/Token.java $(BUILD_DIR)/TokenType.java
	$(JCC) $(JFLAGS) $(BUILD_DIR)/Lox.java $(BUILD_DIR)/Scanner.java $(BUILD_DIR)/Token.java $(BUILD_DIR)/TokenType.java

clean:
	$(RM) $(BUILD_DIR)/*.class
