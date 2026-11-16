# zebrafish-cortisol-development

This is the parent repository for the final project for the fall 2026 semester of BIOL343. To embark on this project, fork the repository and edit it as you please. Grading specifications are described below.

## Tasks

You have been provided with 192 FASTQs filles in `/data/classes/2026/fall/biol343_001/_course_files/30-1264854506/00_fastq`. These reads originated from 16 different samples: wild-type (AB) or knockout (fmr1) zebrafish embryos at 1, 2, 3, and 5 days post-fertilization, treated with either cortisol or vehicle. The goal of this experiment is to analyze whether cortisol treatment has different effects on development in zebrafish carrying a knockout mutation in a gene linked to Fragile X syndrome in humans.

>[!TIP]
> You may want to re-read ["Cortisol-treated zebrafish embryos develop into pro-inflammatory adults with aberrant immune gene regulation."]([https://journals.plos.org/plospathogens/article?id=10.1371/journal.ppat.1012268](https://pubmed.ncbi.nlm.nih.gov/27444789/)). Our project is a follow up to that study.

## Grade specifications

### C

To receive a C in this class, the following are required:

1. The full analysis in a Jupyter notebook that allows reproduction of the entire analysis. At least two plots (PCA of samples and volcano plot of DEGs) should be included. The analysis should include QC evaluation of:
      1. RNA extraction and library prep,
      2. reads before and after trimming,
      3. alignment,
      4. counting,
      5. PCA clustering, and
      6. differential expression.  
  > [!TIP]  
  > This means that you should include Markdown explaining and evaluating logs and QC metrics, as well as your thought process behind each command and argument.
2. An `environment.yaml` file that includes the specifications for generating a conda environment to use as the kernel for the IPython notebook.  
3. A single MultiQC report that includes QC from each command in the notebook.  
4. All of the associated data. Some of it may be too large to put on GitHub, but the count matrices volcano and PCA plots should be included at the very least.
5. An updated README that explains the structure of the repository.  

  > [!IMPORTANT]  
  >The notebook should be organized, written, and formatted in a professional manner, as if you were going to provide it to a client. A rubric will be provided soon.

### B

To receive a B in this class, you are required to do everything required for a C, as well as the following:

1. Use git to version control the entire analysis. Commit messages should be ***informative***, and there should be at least one commit per remaining week of the semester, which means >4 commits.  

### A

To receive an A in this class, you are required to do everything required for a B and C, as well as the following:

1. A snakefile that allows complete reproduction of the analysis. This should be in the `pipeline/` directory.  

## Other details

- Since the FASTQs are provided, you don't need an SRARunTable or to fetch any FASTQs.  
- The reads are paired-end, so your code from the previous homework/notebooks will need to be updated accordingly.

## Using this repository

This repository is a **template**. Using the template gives you a copy that's fully yours: it lives in your personal GitHub account, it doesn't depend on access to this organization, and you can make it public for your portfolio.

1. At the top right of this page, click **Use this template** → **Create a new repository**.
2. Under **Owner**, choose your personal GitHub account (not UWEC-Bioinformatics). You can keep the name `zebrafish-cortisol-development` or rename it.
3. Choose **Public** or **Private**. If you choose Private, go to **Settings** → **Collaborators** in your new repository and add `wheelern` so your work can be graded.
4. Click **Create repository**.
5. Clone your new repository onto BOSe and work inside it:

```
git clone git@github.com:{your username}/zebrafish-cortisol-development.git
cd zebrafish-cortisol-development
```
