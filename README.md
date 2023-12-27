## Varroa Detector

This repository contains the code for the paper *Analysis of Varroa mite colony infestation level using new open software based on deep learning techniques* 
by Jose Divasón, Ana Romero, Francisco Javier Martínez de Pisón, Miguel A. Silvestre, Pilar Santolaria and Jesús L. Yániz.

[This Zenodo entry](https://zenodo.org/doi/10.5281/zenodo.10231844) contains the original dataset, the improved images after applying deblurGAN and the developed
models.

This repository contains two important Jupyter notebooks:
- **train_varroa_mite_detector.ipynb:** this file allows one to reproduce the experiments presented in the paper by choosing
  different models and combination of hyperparameters (crops, weights, threshold confidence, number of epochs, enable deblurGAN, batch size, ...).
- **refinement_step.ipynb:** this file includes the code to perform the refinement step to obtain better bounding boxes. It also includes the benchmarking about the performance of the best models with and without the refinement step and deblurGAN.

Further details can be found in the corresponding files. The experiments have been performed on a computing server with Nvidia RTX 3090 GPUs.

Additionally, one can try the smallest developed model in [Google Colab](https://colab.research.google.com/drive/1KbMLu995LbXHFWO2FpvGYPNRp-OfB_Kq) (note that that the free version of Google Collaboratory is usually rather slow).


