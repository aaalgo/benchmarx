BenchmarX
=========

# Introduction 

The goal of this project is to curate the local evaluation
environment for common deep-learning benchmarks/competitions.

# Organization

Each dataset consists a sub-directory named after the dataset.  In side
that directory, there should be a script `eval.sh` or `eval.py`, or in
the presence of sub-challenges `eval_xxx.sh` or `eval_xxx.py`.  Such
script should typically take in a single parameter, which points to a
file or a directory, which follows the competition's submission format.
The evaluation script should be programmed in such a way that it can be
run from any directory.  Please follow the example of
`kitti/eval_obj.py` on how to locate our own code and data.

# Setup

- Install dependencies: `sudo ./install_deps.sh`
- Build submodules: `make`

