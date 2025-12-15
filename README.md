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

1. Set your working directory to the folder where you saved the file:
   ```r
   gedwd()
   setwd("path/to/your/working/directory")

install.packages("RBiotools_0.5.5.tar.gz", repos = NULL, type = "source")


   library(RBiotools)

