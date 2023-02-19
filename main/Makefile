#hello_exec: hello.cpp
	#g++ hello.cpp -o hello_exec

# Makefile for C++ project

# Define the name of the output executable
EXECUTABLE = PES1UG20CS441-1

# Define the compiler to use
CXX = g++

# Define the compiler flags
CXXFLAGS = -std=c++11 -Wall -Wextra

# Define the source files
SOURCES = hello.cpp

# Define the object files
OBJECTS = $(SOURCES:.cpp=.o)

# Define the Build stage target
build: $(EXECUTABLE)

$(EXECUTABLE): $(OBJECTS)
	$(CXX) $(CXXFLAGS) $^ -o $@

%.o: %.cpp
	$(CXX) $(CXXFLAGS) -c $< -o $@

# Define the Test stage target
test: $(EXECUTABLE)
	./$(EXECUTABLE)

# Define the Deploy stage target
deploy: $(EXECUTABLE)
	@echo "PES1UG20CS441"

# Define the clean target
clean:
	rm -f $(EXECUTABLE) $(OBJECTS)
