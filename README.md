# Offline Policy Evaluation: Counterfactual Estimator
This repo is to reproduce the result of Doubly Robust Estimator.


## Dataset: `./data/*`
|   Dataset   | Samples | Features | Labels |
|:-----------:|:-------:|:--------:|:------:|
|       ecoli |     336 |        7 |      8 |
|       glass |     214 |        9 |      6 |
|      letter |   20000 |       16 |     26 |
|   optdigits |    5620 |       64 |     10 |
| page_blocks |    5473 |       10 |      5 |
|   pendigits |   10992 |       16 |     10 |
|    satimage |    6435 |       36 |      6 |
|     vehicle |     846 |       18 |      4 |
|       yeast |    1484 |        8 |     10 |

**All data can be found under [UCI's great repositories](https://github.com/Rowing0914/offline_policy_evaluation/blob/master/data/README.md)

## Results
- [Bias](https://github.com/Rowing0914/offline_policy_evaluation/blob/master/results/result_bias.txt): `./results/result_bias.txt`
- [RMSE](https://github.com/Rowing0914/offline_policy_evaluation/blob/master/results/result_rmse.txt): `./results/result_rmse.txt`


## Usage
- Get dependencies: `pip install -r requirements.txt`
- Run the main file: `python main.py`


## Dependencies
- Python: 3.6.8
- Packages: See `./requirements.txt`
- OS: Windows10, MacOS, Ubuntu(18.04 LTS)


## TODO
- Fuse the evaluation metrics of OPE by Mix and Rank!!


## Reference
- [IPS/IS](http://www.stat.cmu.edu/~brian/905-2008/papers/Horvitz-Thompson-1952-jasa.pdf)
    - [Capped IPS/IS](https://www.microsoft.com/en-us/research/wp-content/uploads/2013/11/bottou13a.pdf)
    - [Self Normalised IPS/IS](https://www.cs.cornell.edu/people/tj/publications/swaminathan_joachims_15d.pdf)
    - [Pointwise IPS](https://arxiv.org/pdf/1801.07030.pdf)
- [Doubly Robust](https://arxiv.org/abs/1103.4601)
    - [SWITCH](https://arxiv.org/pdf/1612.01205.pdf)
    - [Continuous Adaptive Blending](http://proceedings.mlr.press/v97/su19a/su19a.pdf)
- [Mix and Rank: A Framework for Benchmarking Recommender Systems](https://ieeexplore.ieee.org/document/9006199) 