# Enhancing MRI Images Using Deep Learning

This project implements the U-Net deep learning architecture, and applies the model to the task of enhancing MRI images with under sampled k-spaces. The [fastMRI](https://fastmri.org/dataset/) dataset was used to train and evaluate the effectiveness of the model.

The reconstructed images generated from this model can be found [here](https://drive.google.com/drive/folders/16lBroxjaL8ddR0JEkRKtX4lUuWYkfdZ3?usp=sharing).

This project was undertaken for my MSc Advanced Computer Science, receiving a Distinction grade.

## Prerequisites

The project was built using Python 3.8, and so version 3.8 or later is required to run the project. The following libraries were utilised and are also required for the project to run:

- [Jupyter Notebook](https://jupyter.org)
- [SciPy](https://www.scipy.org)
- [Numpy](https://numpy.org)
- [Matplotlib](https://matplotlib.org)
- [PyTorch](https://pytorch.org)
- [Scikit-image](https://scikit-image.org)
- [H5PY](https://www.h5py.org)

The [fastMRI](https://fastmri.org/dataset/) dataset will also be required to run the project.

## How To Use

The project simply requires a jupyter notebook server to be run, this can be achieved by running the following command in the project directory (or any parent directory):

```
jupyter notebook
```

Then, simply navigate to the [u_net.ipynb](u_net.ipynb) file to run the project. Once opened, run the notebook cells in order. The notebook contains elements of the corresponding paper submitted alongside the code, discussing the method and results step by step.

## Results

Shown below are three different graphs which detail the loss obtained by the project at each epoch of training. The three metrics used to evaluate loss were the mean squared error, L1 norm, and SSIM (note that the implementation of SSIM used computes similarity based on three-dimensional volumes rather than two-dimensional slices).

![L1](img/L1_loss.png =600x )

![MSE](img/MSE_loss.png =600x )

![SSIM](img/SSIM_loss.png =600x )



## License

This project is licensed under the terms of the [Creative Commons Attribution 4.0 International Public license](License.md).