##############################################################
#IMAGE RUNNING SYNTAX: 
# docker run --cap-add=SYS_PTRACE --security-opt seccomp=unconfined -v $(pwd):/workspace -it daa82/gdb-katacoda /bin/bash
##############################################################
from ubuntu:latest

run apt-get update && apt-get upgrade -y
run apt-get install -y build-essential gcc-multilib gdb
run apt-get install -y emacs

#copy
COPY .gdbinit /root/.gdbinit

run mkdir /workspace
workdir /workspace

#create a sample file to test
run echo "int main() { return 0; }" > main.c
run gcc main.c -g -o main

