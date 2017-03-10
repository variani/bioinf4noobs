# MacOS

Download the source code at http://cnsgenomics.com/software/gcta/download.html: `gcta_1.26.0_src.zip`

`HowToCompile.txt`:

> GCTA uses and links two external numerical libraries, i.e. EIGEN and Intel MKL.

## Install Eigen

http://brewformulas.org/Eigen

```
brew install eigen
```

## Install MKL

`HowToCompile.txt`:

>Intel MKL is a commercial library
>http://software.intel.com/en-us/intel-mkl
>However, there is an opportunity to obtain the Intel MKL library (for Linux)
>free of charge for non-commercial use
>http://software.intel.com/en-us/non-commercial-software-development
>I can simply follow the installation instruction to install the library. One
>example of the installation instruction can be found at
>http://software.intel.com/en-us/articles/intel-mkl-103-install-guide

- Get free downloads for Academia: https://software.intel.com/en-us/qualify-for-free-software/academicresearcher
  - A `dmg` file is provided for MacOS
  - Proposed installation path: `/opt/intel/`

## Install gcta

`HowToCompile.txt`:

>Once both EIGEN and Intel MKL libraries have been installed, you can simply
>type the following command to compile GCTA.
>make EIGEN_PATH="your EIGEN library path" MKL_PATH="your Intel MKL library
>path"
>
>For example, if EIGEN library files are in the “eigen-eigen-36bf2ceaf8f5”
>directory under “gcta” directory and Intel MKL library files are install in
>the “/opt/intel/mkl” directory, you can type the command
>make EIGEN_PATH="../eigen-eigen-36bf2ceaf8f5" MKL_PATH="/opt/intel/mkl"
>
>If you can successfully compile the program, you will be able to get an
>executable file called “gcta64” in your working directory (“gcta” directory).

Dependencies paths:

- `/usr/local/opt/eigen/`
- `/opt/intel/`

Command:

```
make EIGEN_PATH="/usr/local/opt/eigen/" MKL_PATH="/opt/intel/mkl"
```

## Caveats

```
clang: error: unsupported option '-fopenmp'
```

http://stackoverflow.com/a/29109926

```
brew reinstall -v gcc --without-multilib
```
