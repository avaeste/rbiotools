https://download1.rstudio.org/electron/windows/RStudio-2025.09.2-418.exe

https://cran.r-project.org/bin/windows/base/R-4.5.2-win.exe

https://cran.r-project.org/bin/windows/Rtools/rtools42/files/rtools42-5355-5357.exe

file.edit("~/.Renviron")

PATH="C:/rtools42/usr/bin;C:/rtools42/x86_64-w64-mingw32.static.posix/bin;${PATH}"

#Add above path to environ file, restart R

Sys.which("make") # should show path now

install.packages('RCurl') 

install.packages("rmarkdown")

install.packages("ape")

install.packages("data.table")

install.packages("fmsb")

install.packages("ggplot2")

install.packages("gplots")

install.packages("grImport")

install.packages("gridExtra")

install.packages("pheatmap")

install.packages("rentrez")

install.packages("seqinr")

install.packages("BiocManager", repos ="http://cran.us.r-project.org")

library(BiocManager)

BiocManager::install("msa", force = TRUE)

BiocManager::install("Biostrings", force = TRUE)

library(msa) # hit n for update none

library(Biostrings) # hit n for update none

### Download RBioTools 
  From this GitHub repository, download:
  - `RBiotools_0.5.6.tar.gz`    
  Click the file, then **Raw**, and save it in your working directory.

setwd("C:/Users/guild/Downloads") # where your 0.5.6 file is / your working dir

install.packages("RBiotools_0.5.6.tar.gz", repos = NULL, type = "source" , quiet = TRUE, verbose = FALSE)

library(RBiotools)

eColi <- c("AP012306","U00096","CP000802","CP000800","AP009378",
           "FM180568","CU928163","CP008957","CP027027","CP026802","CP026877",
           "CP026793","CP015831")

invisible(suppressWarnings(suppressMessages(dendrogram16S(eColi)))) # downloading

# hit zoom button

createAtlas(eColi[1]) # it is saved in your working dir

plotUsage(eColi[1]) # hit zoom button

plotHeatMapCodon(eColi) # it is saved in your working dir


