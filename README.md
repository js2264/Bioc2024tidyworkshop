# Applying tidy principles to investigating chromatin composition and architecture

*Authors:*
    Jacques Serizay^[[Institut Pasteur, Paris](https://research.pasteur.fr/en/team/spatial-regulation-of-genomes/)],
    <br/>
*Last modified:* 2024-07-06.

## Overview

The integration of tidy tools into genomics analysis catalyzes a paradigm shift 
in the way genomicists approach data manipulation and interpretation. 
By adhering to the principles of tidy data organization and the elegant syntax 
of `tidyverse` packages, researchers can navigate the complexities of genomic 
datasets with unprecedented ease and efficiency. 
In this workshop, we will discover two recent packages: 

- `plyinteractions`, specifically developed to manipulate chromatin 
conformation capture (3C, Hi-C micro-C, etc); 
- `tidyCoverage`, to manipulate and extract coverage tracks within the `tidyomics` framework. 

`plyinteractions` and `tidyCoverage` packages introduce novel 
`SummarizedExperiment`-derived S4 classes to store genomics data and expand 
tidy methods, following the principles defined in `plyranges` and
`tidySummarizedExperiment`.  
They synergize the existing functionalities of `tidyverse` and 
Bioconductor, to seamlessly intertwine data manipulation, aggregation, 
visualization, and modeling within a unified framework.  

### Participation

This 90min-long workshop will include brief overview of some of the state-of-the-art packages 
following the `tidyomics` ecosystem recommendations. Most of the workshop will 
be based on a combination of instructor-led live demo and hands-on guided exercises. 

### Pre-requisites

* Knowledge of `GenomicRanges` and `SummarizedExperiment` classes of object
* Familiarity with standard genomic processed data formats (e.g. `bed` files, `bigwig` files, ...)

The following resources are relevant to this workshop: 

* [tidyomics Nat. Methods paper](https://www.nature.com/articles/s41592-024-02299-2)
* [plyranges Genome Biol. paper](https://genomebiology.biomedcentral.com/articles/10.1186/s13059-018-1597-8)
* [tidyCoverage Bioinformatics paper (in press)](https://www.biorxiv.org/content/10.1101/2024.01.27.577537v1)

### _R_ / _Bioconductor_ packages used

- `plyranges`
- `plyinteractions`
- `tidyCoverage`

### Time outline

| Activity                                   | Time |
|--------------------------------------------|------|
| Manipulating genomic ranges data           | 10m  |
| Manipulating genomic interaction data      | 35m  |
| Manipulating coverage data                 | 25m  |
| Putting everything together!               | 20m  |

### Workshop goals and objectives

*Learning goals*: 

- Manipulate genomic features, genomic interactions and/or genomic tracks using `tidyomics` principles;
- Integrating different levels of genomic information together.

*Learning objectives*: 

- Import/coerce genomic features and/or interactions into relevant Bioconductor classes; 
- Summarize genomic information using tidy data approaches; 
- Visualize and aggregate genomic coverage data over genomic features of interest in a tidy manner. 

## Workshop environment 

The companion website for this workshop is available here: 

[https://js2264.github.io/Bioc2024tidyworkshop](https://js2264.github.io/Bioc2024tidyworkshop)

To use the workshop image:

```sh
docker run -e PASSWORD=<choose_a_password_for_rstudio> -p 8787:8787 ghcr.io/js2264/bioc2024tidyworkshop:latest
```

Once running, navigate to http://localhost:8787/ and then login with `rstudio`:`yourchosenpassword`. 
