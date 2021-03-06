## References

Videos

* [All in the genes, or in all the genes](http://www.lshtm.ac.uk/newsevents/multimedia/inaugurallectures/2015/all_in_genes_lecture.html)

Tutorials

* Courses by Aulchenko http://mga.bionet.nsc.ru/~yurii/courses/
  * Example: http://mga.bionet.nsc.ru/~yurii/courses/esp292014/

Benchamrks

* https://github.com/MicrosoftGenomics/GWAS_benchmark

Methodology

* [Diverse convergent evidence in the genetic analysis of complex disease: coordinating omic, informatic, and experimental evidence to better identify and validate risk factors](http://www.biodatamining.org/content/7/1/10)
* [Progress and promise in understanding the genetic basis of common diseases](http://www.ncbi.nlm.nih.gov/pubmed/26702037)
  * [must consider](https://twitter.com/moorejh/status/681493073600233472)  "polygenic analyses...including modest effects..not individually statistically significant"

## Tools

### Ultra-fast R package Matrix_eQTL

http://www.bios.unc.edu/research/genomic_software/Matrix_eQTL/

* Proposed for eQTL mapping
* Official tool of the GTEx project external link 
* Used by seeQTL browser external link
* Basis of Multiple Tissue eQTL

Implementation

* Data are stored in plain text files, but the read out is optimized by slicing via `SlicedData` class of the package
* The file format is row-based, i.e. each row is a sample. That is different from SOLAR files.


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
