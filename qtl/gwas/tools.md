
## References

Groups

* Marchini's group, http://www.stats.ox.ac.uk/~marchini/software/gwas/gwas.html

## VEGAS2

### Installation

1. Install perl libraries
2. Configure
    * remove some DB files to save space on disk
3. Copy exec to path

1) Install perl library `Data::UUID` via https://community.opmantek.com/display/NMIS/Installing+Perl+Libraries+with+and+without+CPAN

Go into:

```
cpan
```

Run there:

```
install Data::UUID
```

2) Configure

```
./vegas2.config /home/andrey/tools/VEGAS2/VEGAS2database /home/andrey/tools/VEGAS2/VEGAS2scripts
```

```
$ ls VEGAS2database/1000GEURO/
0kbloc  1000GEURO.extract  50kbloc
```

3) Install

```
sudo cp vegas2 /usr/local/bin/
```


## Gemma

* https://github.com/vforget/gemma-pipeline
