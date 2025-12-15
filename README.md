# RBioTools

**RBioTools** is an R package for **comparative microbial genomics**.  
It works best in **RStudio** and uses **GenBank (NCBI) IDs** to perform analyses and generate figures.

---

## Installation

### Requirements

- **R**: https://www.r-project.org  
- **RStudio Desktop**: https://posit.co/download/rstudio-desktop  

#### System tools (required to compile R packages)

- **Windows**: Install **Rtools42**  
  https://cran.r-project.org/bin/windows/Rtools/rtools42/rtools.html

  Rtools must match your R version. In R, run: R.version.string
  Verify Rtools installation:
  Sys.which("make")
  
  install.packages("pkgbuild")


---

### Set up working directory

Create a folder on your computer where you will store your work (e.g., `RBioTools`).  
This will be your **working directory**.

---

### Download RBioTools

From this GitHub repository, download:

- `RBiotools_0.5.6.tar.gz`  

Click the file, then **Raw**, and save it in your working directory.



---

### Open RStudio
   ```r
install.packages("rmarkdown")
install.packages(c("ape", "data.table", "fmsb", "ggplot2", "gplots", "grImport", "gridExtra", "pheatmap", "rentrez", "seqinr"))
if (!requireNamespace("BiocManager", quietly = TRUE))
      install.packages("BiocManager", repos ="http://cran.us.r-project.org")

  BiocManager::install("msa", force = TRUE)
  BiocManager::install("Biostrings, force = TRUE)
  install.packages("installr", repos ="http://cran.us.r-project.org")
library(msa) 

library(installr) 

1. Set your working directory to the folder where you saved the file:
   ```r
   gedwd()
   setwd("path/to/your/working/directory")

install.packages("RBiotools_0.5.6.tar.gz", repos = NULL, type = "source")

   library(RBiotools)

