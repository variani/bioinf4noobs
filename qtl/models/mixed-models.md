## Tools

1) [warpedlmm](https://github.com/PMBio/warpedLMM/blob/master/warpedlmm/)

* Specially designed for exploring trait transformations (based on FaST-LMM)
* Paper http://arxiv.org/pdf/1402.5447.pdf
* Equation
      * $z ~ (Xb, sigma_g^2 K + sigma_e^2 K)$
      * $K = (1/S) G G^T$, where G is $N x S$ matrix of S common SNPs used to estimate the relatedness
* Presentations (few new things)
      * http://www2.warwick.ac.uk/fac/sci/statistics/staff/academic-research/nichols/research/neuro-stat/slides_habib.pdf
      * http://www.stage.utoronto.ca/wp-content/uploads/2014/10/MH_ASHG-2014-meeting-highlights.pdf

2) [limix](https://github.com/PMBio/limix)

* Tutorials https://github.com/PMBio/limix-tutorials

3) GCTA

http://cnsgenomics.com/software/gcta/

Issues

* Usage in the family data: http://gcta.freeforums.net/thread/17/variance-explained-family-data
          * Answer: See [article](http://journals.plos.org/plosgenetics/article?id=10.1371/journal.pgen.1003520)

4) FAST-LMM

* Implementations
     * Jilia: https://github.com/sens/FaSTLMM.jl

## Extensions

### MERF

Mixed Effects Trees and Forests for Clustered Data (Mixed Trees and Forests)

* http://www2.ims.nus.edu.sg/Programs/014swclass/files/denis.pdf
    * Overview of stat. methods on clustered data analysis  http://www.jneurosci.org/content/30/32/10601.full?sid=91a1d4ff-c316-402d-a73c-b6c1733ad012

Application to QTL mapping

* 

Implementations

* Building a regression Tree with R FROM SCRATCH
     * https://cran.r-project.org/web/packages/partykit/index.html
          * https://cran.r-project.org/web/packages/partykit/vignettes/partykit.pdf
          * https://cran.r-project.org/web/packages/partykit/vignettes/constparty.pdf
* Introductory materials
     * http://scikit-learn.org/stable/modules/tree.html
     * http://www.stat.cmu.edu/~cshalizi/350/lectures/22/lecture-22.pdf
