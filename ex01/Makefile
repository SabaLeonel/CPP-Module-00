# Updated Makefile for the phonebook project

# Name of your executable
TARGET = phonebook

# Compiler to use
CXX = g++

# Compiler flags
CXXFLAGS = -Wall -Wextra -Werror -std=c++98 -pedantic -g

# Source files
SRC = Main.cpp \
 Phonebook.cpp \
 Contact.cpp

# Object files
OBJ = $(SRC:.cpp=.o)

# Build target
all: $(TARGET)

$(TARGET): $(OBJ)
	$(CXX) $(CXXFLAGS) $(OBJ) -o $(TARGET)

%.o: %.cpp
	$(CXX) $(CXXFLAGS) -c $< -o $@

clean:
	rm -f $(OBJ)

fclean: clean
	rm -f $(TARGET)

re: fclean all

# Phony targets
.PHONY: all clean re fclean
