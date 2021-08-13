# Get the GCC preinstalled image from Docker Hub
FROM gcc:latest

# Copy the current folder which contains C++ source code to the Docker image under /usr/src
# COPY . /usr/src/dockertest1
#COPY . .

# Specify the working directory
#WORKDIR /usr/src/dockertest1
COPY . /cpp-action1
WORKDIR /cpp-action1/

# Use GCC to compile the Test.cpp source file
RUN g++ -o Test Test.cpp

# Run the program output from the previous step
ENTRYPOINT ["/cpp-action1/Test"]
