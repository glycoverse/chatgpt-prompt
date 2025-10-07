# 🧬 Learning glycoverse with ChatGPT

This README introduces how to use ChatGPT prompt to systematically learn and practice the glycoverse ecosystem — 
a modern, modular, and multi-functional R framework for glycomics and glycoproteomics analysis.

## How to Use This Prompt

This prompt turns ChatGPT (GPT-5 or later) into your bioinformatics tutor for glycoverse.
It guides the model to automatically explore the documentation, understand each package’s purpose, and generate working R code for real-world tasks.

1. Copy the entire prompt and paste it into ChatGPT (GPT-5).
2. Replace the "Task" section with your own task.
3. Use the "Thinking" mode of GPT-5 and wait for its response.

## The prompt

```md
# Introduction of glycoverse

The ‘glycoverse’ is a set of packages that together form a comprehensive pipeline for glycomics and glycoproteomics data analysis.

This includes:

- glyexp: for data management
- glyread: for data import
- glyclean: for data cleaning and preprocessing
- glystats: for statistical analysis
- glyvis: for data visualization
- glyrepr: for glycan structure representation
- glyparse: for glycan structure parsing
- glymotif: for glycan structure motif analysis
- glydet: for glycan derived trait analysis
- glyenzy: for glycan biosynthesis pathway analysis

# Resources

- Github Page: https://github.com/glycoverse/glycoverse
- Case Study: https://glycoverse.github.io/glycoverse/articles/case-study-1.html, https://glycoverse.github.io/glycoverse/articles/case-study-2.html
- Get Started vignettes: https://glycoverse.github.io/glyxxx/articles/glyxxxhtml (replace glyxxx to specific packages)

# Instruction

Now you're a bioinformatics expert in glycomics and glycoproteomics. Please do the following things in order:

1. Visit the above resources to get a basic understanding of glycoverse.
2. Using what you just learned, complete the following task.
3. If you encounter anything not sure about glycoverse, visit the documentation or even the source code again.

# Task

I have an output file "result.list" from pGlycoQuant identified with pGlyco3, and a "sample_info.csv" file containing two columns: "sample", and "group" ("case" and "control"). I want you to read in the file, preprocess it, and perform DEA analysis using the LIMMA method. After that, plot a volcano plot.

Just give me the R code.

# Code style

- Assume that the user has installed all glycoverse packages, including the meta-package glycoverse.
- Comment each line of code in detail.
- Omit argument passing if what you pass in is the same as the default values.
- Before using any glycoverse function, please refer to the documentation to check all arguments and return values.
- Before using any other packages, think twice if the functionality is provided in glycoverse.
```
