This is the PyTorch implementation of [ColorMedGAN: A Semantic Colorization Framework for Medical Images](https://www.mdpi.com/2076-3417/13/5/3168)

Abstract : Colorization for medical images helps make medical visualizations more engaging, provides better visualization in 3D reconstruction, acts as an image enhancement technique for tasks such as segmentation, and makes it easier for non-specialists to perceive tissue changes and texture details in medical images in diagnosis and teaching. However, colorization algorithms have been hindered by limited semantic understanding. In addition, current colorization methods still rely on paired data, which is often not available for specific fields such as medical imaging. To address the texture detail of medical images and the scarcity of paired data, we propose a self-supervised colorization framework based on CycleGAN(Cycle-Consistent Generative Adversarial Networks), treating the colorization problem of medical images as a cross-modal domain transfer problem in color space. The proposed framework focuses on global edge features and semantic information by introducing edge-aware detectors, multi-modal discriminators, and a semantic feature fusion module. Experimental results demonstrate that our method can generate high-quality color medical images.

![](https://www.mdpi.com/applsci/applsci-13-03168/article_deploy/html/images/applsci-13-03168-g001-550.jpg)
![](https://www.mdpi.com/applsci/applsci-13-03168/article_deploy/html/images/applsci-13-03168-g002-550.jpg)

# Results

![](https://www.mdpi.com/applsci/applsci-13-03168/article_deploy/html/images/applsci-13-03168-g009-550.jpg)

# Requirements

* torch>=1.0.0
* CUDA toolkit 10.2 or later. 

# Datasets

* [ the Brain MRI dataset Brats2018](https://pubmed.ncbi.nlm.nih.gov/25494501/)
* [The Human Project](https://onlinelibrary.wiley.com/doi/10.1002/(SICI)1097-0185(199804)253:2%3C49::AID-AR8%3E3.0.CO;2-9)
* [The Korean Human Project](https://pubmed.ncbi.nlm.nih.gov/16506204/)


# Install

    pip install -r auton-survival-leftright\requirements.txt

# Run

    python colorCycleGAN\colorization.py


# Citation

> @article{chen2023colormedgan,
  title={ColorMedGAN: A Semantic Colorization Framework for Medical Images},
  author={Chen, Shaobo and Xiao, Ning and Shi, Xinlai and Yang, Yuer and Tan, Huaning and Tian, Jiajuan and Quan, Yujuan},
  journal={Applied Sciences},
  volume={13},
  number={5},
  pages={3168},
  year={2023},
  publisher={MDPI}
}