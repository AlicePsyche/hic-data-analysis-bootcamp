# Hi-C Data Analysis Bootcamp

> A tutorial on measuring, analyzing, and visualizing the 3D genome with Hi-C provided by Harvard, MIT, and UMassMed.

![Funky Colormaps](/teaser.jpg?raw=true "Some funky colormaps")

**📢 Slides, code, and data is available for you to rerun the analyses!** 

## Introduction

4D Nucleome Data Coordination and Integration Center and the Center for 3D Structure and Physics of the Genome hosted a Hi-C data analysis bootcamp at Harvard Medical School on May, 8th 2018. This repo contains the material for this bootcamp. Below, you can find more information on how to walk through the hands-on sessions offline.

## Files in this repository

* **Tutorial Part 1 (Hi-C Protocol)**: [Slides PDF](./HiC-Protocol.pdf) | [PPTX](./HiC-Protocol.pptx)
* **Tutorial Part 2 (From fastqs to contact matrices)**: [Slides HTML](https://hms-dbmi.github.io/hic-data-analysis-bootcamp/)
* **Tutorial Part 3 (From contact matrices to biology)**: [Slides PDF](./From-Contact-Matrix-to-Biology.pdf) | [PPTX](./From-Contact-Matrix-to-Biology.pptx)
* **Tutorial Part 4 (Hi-C Data Visualization - HiGlass)**: [Slides HTML](https://hms-dbmi.github.io/hic-data-analysis-bootcamp/#24)
* **Tutorial Part 5 (Hi-C Data Visualization - HiPiler)**: [Slides PDF](./HiPiler-Exploring-HiC-Features-Through-Visual-Decomposition.pdf) | [HTML](https://speakerdeck.com/flekschas/hi-c-data-visualization-with-hipiler)

## Presenters

* Johan Gibcus, Research Instructor, Universy Massachusetts Medical School
* [Nezar Abdennur](http://nvictus.me/), PhD student, MIT
* [Soo Lee](https://compbio.hms.harvard.edu/people/soohyun-lee), Senior Bioinformatics Scientist, Harvard Medical School
* [Peter Kerpedjiev](http://emptypipes.org/about), Postdoctoral Research Fellow, Harvard Medical School
* [Fritz Lekschas](https://lekschas.de/) PhD Student, Harvard University
* [Leonid Mirny](http://mirnylab.mit.edu/) Professor, MIT

## Organizers

* [Burak Alver](https://compbio.hms.harvard.edu/people/burak-alver-0), Scientific Project Manager, Harvard Medical School
* [Nils Gehlenborg](http://gehlenborglab.org/), Assistant Professor, Harvard Medical School
* [Peter Park](https://compbio.hms.harvard.edu/), Professor, Harvard Medical School

## Motivation and Objectives

Due in large part to the explanatory power of chromosome organization in gene regulation, its association with disease and disorder as well as the unanswered questions regarding the mechanisms behind its maintenance and function, the 3D structure and function of the genome are becoming increasingly target of scientific scrutiny. With efforts such as the 4D Nucleome Project and ENCODE 4 already beginning to generate large amounts of data, the ability to analyze and visualize it will be a valuable asset to any computational biologist tasked with interpretation of experimental results.

The objectives of this tutorial are
* To introduce the theoretical concepts related to 3D genome data analysis
* To familiarize participants with the data types, analysis pipeline, and common tools for analysis and visualization of 3D genome data
* To provide a hands on experience in data analysis by walking through some common use cases of existing tools for data analysis and visualization.

After the workshop participants should be able to obtain, process, analyze, and visualize 3D genome data on their own as well as to understand some of the logic, motivation and pitfalls associated with common operations such as matrix balancing and multi-resolution visualization.

The subject matter and practical exercises presented in this tutorial will be accessible to a broad audience. Prior experience with next generation sequencing and the data it produces will be helpful for understanding the subsequent processing steps used to derive contact maps as well as some of the artifacts that can arise during data processing.

The material will be most useful to computational biologists and biologists working on genomics-related topics.

## Student Requirements

 * A server will be set up for students with all the required software.
 * Windows users, please install [Putty (for ssh)](https://www.chiark.greenend.org.uk/~sgtatham/putty/latest.html).

## Agenda

**09:00 - 09:10** Introduction and Overview (Peter Park and Burak Alver, Harvard)

**09:10 - 10:30** Hi-C Protocol (Johan Gibcus, UMass)

**10:30 - 10:45** _Break_

**10:45 - 12:15** From fastqs to contact matrices (Soohyun Lee, Harvard)

**12:15 - 13:00** _Lunch_

**13:00 - 14:00** From contact matrices to biology (Nezar Abdennur, MIT)

**14:00 - 15:00** Hi-C Data Visualization - HiGlass (Peter Kerpedjiev, Harvard)

**15:00 - 15:15** _Break_

**15:15 - 16:00** Hi-C Data Visualization - HiPiler (Fritz Lekschas, Harvard)

**16:00 - 17:00** Keynote Speaker - Leonid Mirny, MIT


## Instructor Bios

### Johan Gibcus

Johan Gibcus is a Research Instructor at the University of Massachussetts Medical School. He has not only used but also refined the Hi-C protocol to answer important biological questions about chromosome organization and replication. Web: [http://www.dekkerlab.org/](http://www.dekkerlab.org/)

### Soo Lee

Soo Lee is a Senior Bioinformatics Scientist in the Department of Biomedical Informatics at Harvard Medical School. She is creating cloud-based pipelines for Hi-C and other genomic data and developing infrastructure for automation of such pipelines as part of the 4D Nucleome Data Coordination and Integration Center. Web: [compbio.hms.harvard.edu/people/soohyun-lee](https://compbio.hms.harvard.edu/people/soohyun-lee)

### Nezar Abdennur

Nezar Abdennur is a PhD candidate in Computational and Systems Biology at MIT. His research focuses on the determinants of 3D genome organization and the development of tools for dealing with large Hi-C datasets. Twitter: [@nv1ctus](https://twitter.com/nv1ctus) Web: [nvictus.me](http://nvictus.me)

### Peter Kerpedjiev

Peter Kerpedjiev is a postdoctoral researcher working on creating tools (such as [HiGlass](http://higlass.io)) for visualizing large genomic data sets. Twitter: [@pkerpedjiev](https://twitter.com/pkerpedjiev) Web: [emptypipes.org](http://emptypipes.org)

### Fritz Lekschas

Fritz is a PhD student working on biomedical information visualization with focus on large multiscale genomic data sets. He created tools like [HiPiler](http://hipiler.lekschas.de) or [Scalable Insets](http://scalable-insets.lekschas.de) Twitter: [@flekschas](https://twitter.com/flekschas) Web: [lekschas.de](https://lekschas.de)

### Leonid Mirny

Leonid Mirny is a professor at MIT's Institute for Medical Engineering & Science. His lab studies the three dimensional organization of chromosomes using a combination of computational analysis and simulation. Twitter: [@leonidmirny](https://twitter.com/leonidmirny) Web: [mirnylab.mit.edu](http://mirnylab.mit.edu/)

## Pointers for Offline Walk-through

During the bootcamp, users were given access to linux servers where
- docker was installed,
- conda was installed,
- a conda enivronment was set up with a number of dependencies
installed, including juypter notebook,
- higlass-manager was installed,
- and sample data was downloaded.

You can set up a similar environment and walk through the hands-on
sessions of the bootcamp by following the instructions below. Allow 30G of storage for all files used in the tutorial.

### From fastqs to contact matrices

1. Install [docker](https://docs.docker.com/install/), if you have not already done so. ([Docker](https://docs.docker.com/) is a lighter alternative to virtual machines.)
2. Pull the docker image: `docker pull duplexa/4dn-hic:v42`. This docker image contains a number of software that have been pre-installed for HiC data processing.
3. Download the sample data for this session under your home directory to "~/data/" (or edit the commands on the slides accordingly, if you prefer a different directory).
```
mkdir data
cd data/
# input fastq files
wget https://s3.amazonaws.com/4dn-dcic-public/hic-data-analysis-bootcamp/input_R1.fastq.gz
wget https://s3.amazonaws.com/4dn-dcic-public/hic-data-analysis-bootcamp/input_R2.fastq.gz
gunzip input_R1.fastq.gz
gunzip input_R2.fastq.gz
# bwa genome index
wget https://s3.amazonaws.com/4dn-dcic-public/hic-data-analysis-bootcamp/hg38.bwaIndex.tgz
tar -xzf hg38.bwaIndex.tgz
rm hg38.bwaIndex.tgz
# chromsizes
wget https://s3.amazonaws.com/4dn-dcic-public/hic-data-analysis-bootcamp/hg38.mainonly.chrom.size
# prebaked output files
wget https://s3.amazonaws.com/4dn-dcic-public/hic-data-analysis-bootcamp/prebaked.tgz
tar -xzf prebaked.tgz
rm prebaked.tgz
# move back a directory
cd ..
```

Now, you should be able to follow slides 1 through 23 of [the tutorial](https://hms-dbmi.github.io/hic-data-analysis-bootcamp/). When you are finished, exit the docker container with `Ctrl-d` before proceeding to the next part.

### Working in a cluster without docker

If you are working in a High Performance Compute Cluster, you may not
be allowed the install Docker. Instead, you can find the recipe for
the docker image used above
[here](https://github.com/4dn-dcic/docker-4dn-hic/tree/v42). The exact configuration of the docker image can be seen in the
[dockerfile](https://github.com/4dn-dcic/docker-4dn-hic/blob/v42/Dockerfile). You
can get information on the  bioinformatics software installed inside the docker image in the [download.sh](https://github.com/4dn-dcic/docker-4dn-hic/blob/v42/downloads.sh)
file.

### From contact matrices to biology

1. Install [conda](https://conda.io/miniconda.html), if you have not
   already done so. Conda is an open source package management tool that allows you to create separate environments.
2. Clone this repo and set up the environment.
    ```
    git clone https://github.com/hms-dbmi/hic-data-analysis-bootcamp
    cd hic-data-analysis-bootcamp
    git pull
    #you may need some of the following in case you have an issue creating an environment
    #conda update --all -y
    #sudo yum install -y hg
    #conda install gcc
    conda env create -n bootcamp -f environment.yml
    ```
3. Download the sample data for this session into the pre-existing "notebooks/data" directory (or edit the commands on the slides accordingly, if you prefer a different directory.
    ```
    # from the hic-data-analysis-bootcamp directory we just made
    cd notebooks/data
    wget https://s3.amazonaws.com/4dn-dcic-public/hic-data-analysis-bootcamp/NIPBL.1000.mcool
    wget https://s3.amazonaws.com/4dn-dcic-public/hic-data-analysis-bootcamp/NIPBL.10000.cool
    wget https://s3.amazonaws.com/4dn-dcic-public/hic-data-analysis-bootcamp/NIPBL.20000.cool
    wget https://s3.amazonaws.com/4dn-dcic-public/hic-data-analysis-bootcamp/NIPBL.40000.cool
    wget https://s3.amazonaws.com/4dn-dcic-public/hic-data-analysis-bootcamp/NIPBL.100000.cool
    wget https://s3.amazonaws.com/4dn-dcic-public/hic-data-analysis-bootcamp/TAM.1000.mcool
    wget https://s3.amazonaws.com/4dn-dcic-public/hic-data-analysis-bootcamp/TAM.10000.cool
    wget https://s3.amazonaws.com/4dn-dcic-public/hic-data-analysis-bootcamp/TAM.20000.cool
    wget https://s3.amazonaws.com/4dn-dcic-public/hic-data-analysis-bootcamp/TAM.40000.cool
    wget https://s3.amazonaws.com/4dn-dcic-public/hic-data-analysis-bootcamp/TAM.100000.cool
    wget https://s3.amazonaws.com/4dn-dcic-public/hic-data-analysis-bootcamp/UNTR.1000.mcool
    wget https://s3.amazonaws.com/4dn-dcic-public/hic-data-analysis-bootcamp/UNTR.10000.cool
    wget https://s3.amazonaws.com/4dn-dcic-public/hic-data-analysis-bootcamp/UNTR.20000.cool
    wget https://s3.amazonaws.com/4dn-dcic-public/hic-data-analysis-bootcamp/UNTR.40000.cool
    wget https://s3.amazonaws.com/4dn-dcic-public/hic-data-analysis-bootcamp/UNTR.100000.cool
    
    wget https://s3.amazonaws.com/4dn-dcic-public/hic-data-analysis-bootcamp/CtcfCtrl.mm9__VS__InputCtrl.mm9.narrowPeak_with_motif.txt.gz
    wget https://s3.amazonaws.com/4dn-dcic-public/hic-data-analysis-bootcamp/GSM1551552_HIC003_merged_nodups.txt.subset.gz
    wget https://s3.amazonaws.com/4dn-dcic-public/hic-data-analysis-bootcamp/NIPBL_R1.nodups.pairs.gz
    wget https://s3.amazonaws.com/4dn-dcic-public/hic-data-analysis-bootcamp/NIPBL_R1.nodups.pairs.gz.px2
    wget https://s3.amazonaws.com/4dn-dcic-public/hic-data-analysis-bootcamp/Rao2014-GM12878-MboI-allreps-filtered.1000kb.cool
    wget https://s3.amazonaws.com/4dn-dcic-public/hic-data-analysis-bootcamp/Rao2014-GM12878-MboI-allreps-filtered.5kb.cool
    wget https://s3.amazonaws.com/4dn-dcic-public/hic-data-analysis-bootcamp/UNTR_R1.nodups.pairs.gz
    wget https://s3.amazonaws.com/4dn-dcic-public/hic-data-analysis-bootcamp/UNTR_R1.nodups.pairs.gz.px2
    wget https://s3.amazonaws.com/4dn-dcic-public/hic-data-analysis-bootcamp/b37.chrom.sizes.reduced
    wget https://s3.amazonaws.com/4dn-dcic-public/hic-data-analysis-bootcamp/ctcf-sites.paired.300kb_flank10kb.tsv
    wget https://s3.amazonaws.com/4dn-dcic-public/hic-data-analysis-bootcamp/hg19.chrom.sizes.reduced
    wget https://s3.amazonaws.com/4dn-dcic-public/hic-data-analysis-bootcamp/mm9.chrom.sizes.reduced
    wget https://s3.amazonaws.com/4dn-dcic-public/hic-data-analysis-bootcamp/mm9.fa
    wget https://s3.amazonaws.com/4dn-dcic-public/hic-data-analysis-bootcamp/ranked_TSS.tsv
    ```
4. Go back to the "notebooks" directory and activate the environment to run the jupyter notebook.
    ```
    cd ..
    source activate bootcamp
    jupyter notebook
    ```
If you're running it on your local machine, the notebook will open at http://localhost:8888. You may have to input the token displayed when starting up the Jupyter. Follow the steps in the notebooks starting with the top one, named "00_intro_cooler-cli".

### HiGlass
1. Install and start docker on your machine.
    ```
    docker pull gehlenborglab/higlass:v0.2.63  # higlass
    pip install higlass-manage --upgrade
    ```
2. Download the sample data.
    ```
    wget https://s3.amazonaws.com/4dn-dcic-public/hic-data-analysis-bootcamp/Schwarzer-et-al-2017-NIPBL.multi.cool
    wget https://s3.amazonaws.com/4dn-dcic-public/hic-data-analysis-bootcamp/Schwarzer-et-al-2017-RNAseq-minus.bw
    wget https://s3.amazonaws.com/4dn-dcic-public/hic-data-analysis-bootcamp/Schwarzer-et-al-2017-UNTR.multi.cool
    ```

Now, you should be able to follow slides 24 through 59 of [the tutorial](https://hms-dbmi.github.io/hic-data-analysis-bootcamp/#24).


## Resources

### Software

* [bwa](https://github.com/lh3/bwa) and [SAM spec](https://samtools.github.io/hts-specs/SAMv1.pdf)
* [pairsamtools](https://github.com/mirnylab/pairsamtools)
* [pairix](https://github.com/4dn-dcic/pairix)
* [cooler](https://github.com/mirnylab/cooler) and [docs](http://cooler.readthedocs.io/en/latest/)
* [HiGlass](http://higlass.io), [source code](https://github.com/hms-dbmi/higlass/), and [docs](https://hms-dbmi.github.io/higlass-docs/)
* [HiPiler](http://hipiler.higlass.io), [source code](https://github.com/flekschas/hipiler), [docs](https://github.com/flekschas/hipiler/wiki), [project page](http://hipiler.lekschas.de)

### Package and environment management

* [conda](https://conda.io/miniconda.html)
* [bioconda](https://bioconda.github.io/)



### Papers

* Imakaev, Maxim, et al. "Iterative correction of Hi-C data reveals hallmarks of chromosome organization." Nature methods 9.10 (2012): 999-1003. doi:[10.1038/nmeth.2148](https://doi.org/10.1038/nmeth.2148)
* Lajoie, Bryan R., Job Dekker, and Noam Kaplan. "The Hitchhiker’s guide to Hi-C analysis: practical guidelines." Methods 72 (2015): 65-75. doi:[10.1016/j.ymeth.2014.10.031](https://doi.org/10.1016/j.ymeth.2014.10.031)
* Kerpedjiev, Peter, et al. "HiGlass: Web-based Visual Comparison And Exploration Of Genome Interaction Maps" bioRxiv. doi:[10.1101/121889](https://doi.org/10.1101/121889)
* Lekschas, Fritz et al. "HiPiler: Visual Exploration Of Large Genome Interaction Matrices With Interactive Small Multiples" IEEE Transactions on Visualization and Computer Graphics, 24(1), 522-531. [doi:10.1109/TVCG.2017.2745978](https://doi.org/10.1109/TVCG.2017.2745978)
* Belaghzal H, et al. "Hi-C 2.0: An optimized Hi-C procedure for high-resolution genome-wide mapping of chromosome conformation." Methods. 2017 [https://doi.org/10.1016/j.ymeth.2017.04.004](https://doi.org/10.1016/j.ymeth.2017.04.004)
* Golloshi R, et al. "Iteratively improving Hi-C experiments one step at a time." Methods. 2018 [https://doi.org/10.1016/j.ymeth.2018.04.033](https://doi.org/10.1016/j.ymeth.2018.04.033)
* Oddes, Sivan, et al. "Three invariant Hi-C interaction patterns: applications to genome assembly". bioRxiv 306076. [https://doi.org/10.1101/306076](https://doi.org/10.1101/306076)
