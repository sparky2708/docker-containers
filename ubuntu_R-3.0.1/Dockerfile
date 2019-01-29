from ubuntu:latest

ENV TZ=US
RUN ln -snf /usr/share/zoneinfo/$TZ /etc/localtime && echo $TZ > /etc/timezone
run apt-get update && apt-get upgrade -y              

run apt-get install build-essential -y
run apt-get install fort77 -y
run apt-get install xorg-dev -y
run apt-get install liblzma-dev  libblas-dev gfortran -y
run apt-get install gcc-multilib -y
run apt-get install gobjc++ -y
run apt-get install aptitude -y
run aptitude install libreadline-dev -y
run apt-get install default-jdk -y
run apt-get install chromium-browser -y
run apt-get install texlive -y
run apt-get install texlive-fonts-extra -y
run apt-get install texinfo -y

run apt-get install wget -y
run wget https://cran.r-project.org/src/base/R-3/R-3.0.1.tar.gz
run tar xvf R-3.0.1.tar.gz
run cd R-3.0.1 && ./configure && make 
run cd R-3.0.1 && make install && make install-info && make install-pdf
run rm R-3.0.1.tar.gz
run rm -rf R-3.0.1

run mkdir /workspace
workdir /workspace
                