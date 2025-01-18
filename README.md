# learn-R

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

3. Download the R source
```bash
export R_VERSION=4.4.2
curl -O https://cran.rstudio.com/src/base/R-4/R-${R_VERSION}.tar.gz
tar -xzvf R-${R_VERSION}.tar.gz
cd R-${R_VERSION}
```









