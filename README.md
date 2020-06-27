## Synthetic Unsupervised pseudo Metric Learning (SUML)
```
Github repository for our AAAI 2020 accepted paper: Unsupervised Metric Learning with Synthetic Examples
```
Link to paper: [Unsupervised Metric Learning with Synthetic Examples](https://www.aaai.org/Papers/AAAI/2020GB/AAAI-DuttaU.7665.pdf) 

In this paper, we use unlabeled data to generate adversarial, synthetic constraints for metric learning. We minimize the entropy of a conditional probability to learn the metric. Our method is called SUML.


### Illustration of SUML
<img src="https://github.com/ukdsvl/SUML/blob/master/illustration/SUML_idea.png?raw=true" width="350">

In the above figure, c represents one of the possbile ordering of examples in a randomly sampled triplet.

## Usage
Firstly, create a conda environment using the provided .yml file. It contains all the necessary requirements.
```
conda env create -f rdml.yml -p <full_path>/<env_name>
```
Activate the conda environment:
```
conda activate <env_name>
```

Refer the jupyter notebook provided here to get an idea of the format of the data that you want to execute your code upon. Mostly, it requires data in the form of ``` dxN ``` matrices, where ```d``` is the dimensionality of the data, and ```N``` is the number of examples.

To extend SUML for the deep setting using PyTorch, the cost provided in the notebook can be used in computing the loss for a mini-batch.

## Citation

If you find the code useful, kindly consider citing our paper:
```
@inproceedings{dutta2020unsupervised,
  title={Unsupervised Metric Learning with Synthetic Examples.},
  author={Dutta, Ujjal Kr and Harandi, Mehrtash and Sekhar, C Chandra},
  booktitle={AAAI},
  pages={3834--3841},
  year={2020}
}
```

Additionally, citation to the Pymanopt paper is:
```
@article{JMLR:v17:16-177,
  author  = {James Townsend and Niklas Koep and Sebastian Weichwald},
  title   = {Pymanopt: A Python Toolbox for Optimization on Manifolds using Automatic Differentiation},
  journal = {Journal of Machine Learning Research},
  year    = {2016},
  volume  = {17},
  number  = {137},
  pages   = {1-5},
  url     = {http://jmlr.org/papers/v17/16-177.html}
}
```
