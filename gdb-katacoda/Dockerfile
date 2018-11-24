#syntax: docker run --cap-add=SYS_PTRACE --security-opt seccomp=unconfined -v $(pwd):/workspace -it daa82/gdb-katacoda /bin/bash
from ubuntu:latest

run apt-get update && apt-get upgrade -y
run apt-get install -y build-essential gdb
run apt-get install -y emacs

run mkdir /workspace
workdir /workspace
