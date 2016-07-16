# VBS

###Installation

##### Requirements:
1. Install htslib

https://github.com/samtools/htslib

2. Perl version: > 5.14.4 
3. Perl packages:
* Getopt::Long::Subcommand
* Bio::DB::HTS::Tabix
```
wget https://raw.githubusercontent.com/miyagawa/cpanminus/master/cpanm
chmod 755 cpanm
./cpanm Getopt::Long::Subcommand
./cpanm Bio::DB::HTS::Tabix
```
4. R version: > 3.3.0

5. R packages
* ggplot2
* pheatmap
Install some required libraries in R:
```
install.packages("ggplot2", dep=T)
install.packages("pheatmap", dep=T)
```

### USAGE
#### ViewBS 

###Appendix: Full list of options

#### 1) Top level commands

```
NAME
       ViewBS - Tools for exploring and visualizing deep sequencing of  bisulfite
        seuquencing (BS-seq) data.

VERSION
       0.2.0

SYNOPSIS

       ViewBS <subcmd> [options]

DESCRIPTION

       ViewBS is developped to mine and visualize bisulfite seuquencing data.

Options
       -help | -h
               Prints the help message and exits.

       -Subcommands:
       -MethGeno
                - Generate the methylation information across each chromosome and plot the information.

       -MethRegion
                - Generate the methylation information across the regions provided here. The regions
                  can be genes, transposable elements, etc.

       -MethHeatmap
                - Generate methylation information for a list of regions in different samples or contexts.

       -MethMidpoint
                - Generate methylation information across the midpoints of a list of regions, like DMR.

HELP
               Here is the discussion group from google group: https://groups.google.com/forum/#!forum/viewbs

Denpendcies
       perl > v5.14.4
       Perl packages
                - Getopt::Long::Subcommand;
                - Bio::DB::HTS::Tabix;

       R  > v3.1.2
       R packages
                - ggplot2;
                - pheatmap

```

####

