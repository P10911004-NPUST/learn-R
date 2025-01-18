# learn-R

3. Download the R source
```bash
export R_VERSION=4.4.2
export INSTALL_PATH='/home/ubuntu/software/R/R-${R_VERSION}'

mkdir -p ${dirname INSTALL_PATH}
cd ${dirname INSTALL_PATH}

wget https://cran.r-project.org/src/base/R-4/R-${R_VERSION}.tar.gz
tar -xzvf R-${R_VERSION}.tar.gz
cd R-${R_VERSION}
```

```bash

cd ${INSTALL_PATH}
```

## Install R from source
1. Install dependencies
```bash
sudo apt-get update
sudo apt-get install -y gfortran
sudo apt-get install -y build-essential
sudo apt-get install -y libreadline-dev
sudo apt-get install -y zlib1g-dev
sudo apt-get install -y libbz2-dev
sudo apt-get install -y libx11-dev
sudo apt-get install -y libcurl4-openssl-dev
sudo apt-get install -y libpng-dev libjpeg-dev libtiff-dev
sudo apt-get install -y liblzma-dev
sudo apt-get install -y libpcre2-dev
sudo apt-get install -y libssl-dev
sudo apt-get install -y libicu-dev
sudo apt-get install -y libblas-dev liblapack-dev
sudo apt-get install -y libcairo2-dev
sudo apt-get install -y libxml2-dev
sudo apt-get install -y default-jdk
sudo apt-get install -y texinfo texlive texlive-fonts-extra
```

4. Configuration
```bash
./configure \
  --prefix=${INSTALL_PATH} \
  --enable-R-shlib \
  --enable-memory-profiling \
  --with-blas \
  --with-lapack

make
```

5. Add system path
```bash
mkdir ~/bin
cd ~/bin
ln -s ${INSTALL_PATH}/bin/R ./R
ln -s ${INSTALL_PATH}/bin/Rscript ./Rscript
ln -s ${INSTALL_PATH}/bin/Rcmd ./Rcmd
```

6. Export PATH in .bashrc file, insert the command at the end of the file
```bash
export PATH='${PATH}:~/bin'
```

7. Source the .bashrc
```bash
source ~/.bashrc
```




