# Temporal Fast Downward

This is slightly modified version of TFD v0.4 (from IPC 2014).


> What is TFD?
> TFD is a temporal planning system that successfully participated in the temporal satisficing track of the 6th International Planning Competition 2008. It is released under the terms of the GPL. A snapshot of the source code is available in the download section.
>
> The algorithms used in TFD are described in the ICAPS 2009 paper [[1]][tfd_paper]. TFD is based on the Fast Downward planning system and uses an adaptation of the context-enhanced additive heuristic [[2]](http://gki.informatik.uni-freiburg.de/papers/helmert-geffner-icaps2008.pdf) to guide the search in the temporal state space induced by the given planning problem.
>
> TFD is mainly developed by Gabriele Röger, Patrick Eyerich, Christian Dornhege, and Robert Mattmüller.

Original Links
* [Homepage][tfd]
* [Downloads][downloads]
* [Contact](mailto:tfd@informatik.uni-freiburg.de)

## Installation

```bash
git clone https://github.com/neighthan/tfd
cd tfd
./build
```

## Usage

```bash
downward/tfd domain_path problem_path solution_path [planner_config]
```

You can find a several benchmark domain and problem files in the `benchmarks` directory. To test your installation, try running

```
downward/tfd benchmarks/openstacks-numericadl/domain.pddl benchmarks/openstacks-numericadl/p01.pddl plan.txt
```
* This should take around 5 minutes to generate an optimal plan. The duration of the optimal plan should be about 82 seconds.
* The planner will periodically output improved plans, numbered sequentially as `plan.txt.1`, `plan.txt.2`, etc. until it times out or finds the optimal plan.

You can add a symlink to `tfd/downward/tfd` from somewhere on your path (e.g. `~/bin`) to run this command from anywhere.

## Modifications
* convert from python 2 to 3 + python formatting changes
* rename `plan.py` to `tfd`, make it robust to running from different directories, delete the intermediate files by default
* don't treat errors as warnings during compilation

## Citation

If you use TFD in your research, please cite

```bibtex
@inproceedings{Eyerich2009UsingTC,
  title={Using the Context-enhanced Additive Heuristic for Temporal and Numeric Planning},
  author={Patrick Eyerich and Robert Mattm{\"u}ller and Gabriele R{\"o}ger},
  booktitle={ICAPS},
  year={2009}
}
```

[tfd]: http://gki.informatik.uni-freiburg.de/tools/tfd/
[tfd_paper]: http://gki.informatik.uni-freiburg.de/papers/eyerich-etal-icaps09.pdf
[downloads]: http://gki.informatik.uni-freiburg.de/tools/tfd/downloads.html
