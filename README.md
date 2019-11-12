fastRPCA
========

Matlab code for all variants of robust PCA and SPCP. This fork includes code for Split-SPCP from the paper "Adapting Regularized Low Rank Models for Parallel Architectures" (Driggs, Becker, Aravkin; SISC 2019). See also "A variational approach to stable principal component pursuit" (Aravkin, Becker, Cevher, Olsen; UAI 2014).

Split-SPCP is generally much faster than other SPCP solvers, and significantly faster than other solvers on the GPU, so it is suitable for extremely large datasets and real-time applications (such as real-time background subtraction). See the [paper for details](https://epubs.siam.org/doi/abs/10.1137/17M1147342?mobileUi=0)


<p align="center"><img src="http://amath.colorado.edu/faculty/becker/escalatorImage.jpg" /></p>


More info on robust PCA and stable principal component pursuit
(websites with software, review articles, etc.)

* ["A variational approach to stable principal component pursuit"](http://arxiv.org/abs/1406.1089)
* [LRS Library](https://github.com/andrewssobral/lrslibrary)
* [Matrix Factorization jungle](https://sites.google.com/site/igorcarron2/matrixfactorizations)
* [One of the first papers on RPCA](http://arxiv.org/abs/0912.3599)


Citation
---------
bibtex (for Split-SPCP):

```
@article{split-spcp2019,
    author       = "Driggs, D. and Becker, S. and Aravkin, A.",
    title        = "Adapting Regularized Low-Rank Models for Parallel Architectures",
    booktitle    = "SIAM J. Sci. Comput.",
    year         = "2019",
}
```

for original code:

```
@inproceedings{aravkin2014,
    author       = "Aravkin, A. and Becker, S. and Cevher, V. and Olsen, P.",
    title        = "A variational approach to stable principal component pursuit",
    booktitle    = "Conference on Uncertainty in Artificial Intelligence (UAI)",
    year         = "2014",
    month        = "July",
}
```

Code and installation
----

The code runs on MATLAB and does not require any mex files or installation. Just unzip the file and you are set. Run `setup_fastRPCA` to set the correct paths, and try the `demos` directory for sample usage of the code.

Authors
--------------
Split-SPCP was implemented by Derek Driggs. The rest of the code was developed by all the authors of the UAI paper, but primary development is due to Stephen Becker and Aleksandr (Sasha) Aravkin. Further contributions are welcome.

