
## References

* http://biology.stackexchange.com/questions/35330/math-behind-the-genetic-relationship-matrix: math behind
* http://www.well.ox.ac.uk/dtc/Genetic%20Analysis.pdf (slide 4): var-covar for a scaled matrix of genotypes (divided by M)
* http://www.xzlab.org/software/GEMMAmanual.pdf: page 20

```
> athaliana::athaliana_compute_relmat
function(snp) 
{
  ### prepare the matrix of genotypes: to be centered / scaled
  mat <- as.matrix(snp[-1])
  mat <- scale(mat, center = TRUE, scale = TRUE)

  ### var
  M <- ncol(mat)
  ids <- snp[["id"]]
  
  ### compute the var-covar matrix
  relmat <- tcrossprod(mat) / M
  
  rownames(relmat) <- ids
  colnames(relmat) <- ids  
  
  return(relmat)
}
<environment: namespace:athaliana>
```

## Tools for computing GRM

R packages

* http://zhengxwen.github.io/SNPRelate/release/help/snpgdsGRM.html: SNP data in GDS format is required
