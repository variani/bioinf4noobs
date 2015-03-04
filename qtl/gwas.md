## References

Benchamrks

* https://github.com/MicrosoftGenomics/GWAS_benchmark


## Tools

### GWASTools

* http://www.maizegenetics.net/#!gapit/cmkv: GAPIT – Genome Association and Prediction Integrated Tool – is an R package that performs Genome Wide Association Study (GWAS) and genome prediction (or selection). This program uses state-of-the-art methods developed for statistical genetics, such as the unified mixed model, EMMA, the compressed mixed linear model, and P3D/EMMAx.
 
1) Install R package ncdf

* http://stackoverflow.com/questions/17028465/installation-of-package-ncdf-fails-due-to-missing-header-although-its-there
* http://cran.fhcrc.org/web/packages/ncdf/INSTALL

1. sudo apt-get install netcdf-bin
2. nc-config --includedir # e.g. output is /usr/include
3. cp /usr/include/netcdf.h .
4. R> install.packages("ncdf")


2) Install R package gdsfmt

https://github.com/zhengxwen/gdsfmt

The install_github() approach requires that you build from source, i.e. make and compilers must be installed on your system – see the R FAQ for your operating system; you may also need to install dependencies manually.

library(devtools)
install_github("zhengxwen/gdsfmt")

### Install R package SNPRelate
