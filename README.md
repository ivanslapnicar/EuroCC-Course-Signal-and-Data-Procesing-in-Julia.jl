# Signal Decomposition, Sparse-plus-low-rank Splitting, and Compressive Sensing in Julia

Lecture notebooks on signal decomposition, sparse-plus-low-rank splitting, and compressive sensing.

Notebooks are written in [Julia](https://julialang.org) using [Pluto.jl](https://github.com/fonsp/Pluto.jl).

Notebooks have been used in the EuroCC on-line workshop (short course)

[AI Techniques: Signal Decomposition, Sparse-plus-low-rank Splitting, and Compressive Sensing in Julia](https://hpc-portal.eu/node/2259).

The notebooks are originally part of the course 

[Modern Applications of Numerical Linear Algebra Methods](https://github.com/ivanslapnicar/GIAN-Applied-NLA-Course).

## Viewing the notebooks

You can view the notebooks at [https://ivanslapnicar.github.io/EuroCC-Course-Signal-and-Data-Procesing-in-Julia.jl](https://ivanslapnicar.github.io/EuroCC-Course-Signal-and-Data-Procesing-in-Julia.jl)

## Running the notebooks

You can run the notebooks in two ways:

### Running on `binder`

1. Go to [https://ivanslapnicar.github.io/EuroCC-Course-Signal-and-Data-Procesing-in-Julia.jl](https://ivanslapnicar.github.io/EuroCC-Course-Signal-and-Data-Procesing-in-Julia.jl) and choose the desired notebook.
2. Press `Edit or run this notebook` button and choose `binder`. This will read all the necessary packages and start the notebook (within several minutes).

### Running on your computer

1. Clone the entire repository by using `Download ZIP` or by using `git` command:
```
git clone https://github.com/ivanslapnicar/Data-Clustering-in-Julia.jl
```
If you are unfamiliar with the `git` tool, check GitHub [help pages](https://help.github.com/articles/set-up-git/). You can also download the repository as a zip file.

2. Install [Julia](https://julialang.org/downloads/). In Julia terminal run the commands
```
> using Pkg
> Pkg.add("Pluto")
> using Pluto
> Pluto.run()
```
This opens local Pluto server in your browser. Now you can choose the notebook and run it
(the notebboks are located in the directory `EuroCC-Course-Signal-and-Data-Procesing-in-Julia.jl/Lectures/`).

## Contents

The lectures are intended for students, scientists, and programmers working in data analysis and artificial intelligence. 
The lectures describe three algorithms used in signal processing and data analysis. 
The algorithms use methods of linear algebra to solve the following problems:

### Signal Decomposition

_Input:_ Suppose we are given a data signal that consists of several nearly mono-components (almost periodic signal where amplitude, frequency, and phase slightly change in time).

_Question:_ Can we recover the mono-components?

_Answer:_ YES, with an efficient algorithm using fast eigenvalue decomposition of Hankel matrices!

_Applications:_ Mono-component recovery can be successfully used to analyse audio signals.


### Sparse + Low-rank Splitting

_Input:_ Suppose we are given a data matrix, and know that it has a form A=L+S, where L is a matrix of low rank and S is a sparse matrix 
(but we know neither the rank nor the location of the non-zero entries).

_Question:_ Can we recover L and S?

_Answer:_ YES, with high probability using an efficient algorithm based on singular value decomposition and iterative thresholding!

_Applications:_ Detecting moving objects in video surveillance, latent semantic indexing, collaborative filtering.


### Compressive Sensing

_Input:_ Several samples of a sparse signal. The number of samples is (far) smaller than the desired signal resolution. 

_Question:_ Can we recover the sparse signal from a few measurements?

_Answer:_ YES, for some signals and carefully selected measurements using l1 minimization (linear programming)!

_Applications:_ Images. 
 


