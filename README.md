# Intrusion-Detection-System-Using-CNN-and-Transfer-Learning

This is the code for the paper entitled "**[A Transfer Learning and Optimized CNN Based Intrusion Detection System for Internet of Vehicles](https://arxiv.org/pdf/2201.11812.pdf)**" published in **IEEE International Conference on Communications (IEEE ICC)**, doi: [10.1109/ICC45855.2022.9838780](https://ieeexplore.ieee.org/document/9838780).  
- Authors: Li Yang and Abdallah Shami  
- Organization: The Optimized Computing and Communications (OC2) Lab, ECE Department, Western University

This repository introduces how to use **convolutional neural networks (CNNs)** and **transfer learning** techniques to develop **intrusion detection systems**. **Ensemble learning** and **hyperparameter optimization techniques** are also used to achieve optimized model performance.

- Another **intrusion detection system development code** using **decision tree-based machine learning algorithms (Decision tree, random forest, XGBoost, stacking, etc.)** can be found in: [Intrusion-Detection-System-Using-Machine-Learning](https://github.com/Western-OC2-Lab/Intrusion-Detection-System-Using-Machine-Learning)

- A comprehensive **hyperparameter optimization** tutorial code can be found in: [Hyperparameter-Optimization-of-Machine-Learning-Algorithms](https://github.com/LiYangHart/Hyperparameter-Optimization-of-Machine-Learning-Algorithms)

## Abstract of The Paper
Modern vehicles, including autonomous vehicles and connected vehicles,  are increasingly connected to the external world, which enables various functionalities and services. However, the improving connectivity also increases the attack surfaces of the Internet of Vehicles (IoV), causing its vulnerabilities to cyber-threats. Due to the lack of authentication and encryption procedures in vehicular networks, Intrusion Detection Systems (IDSs) are essential approaches to protect modern vehicle systems from network attacks. In this paper, a transfer learning and ensemble learning-based IDS is proposed for IoV systems using convolutional neural networks (CNNs) and hyper-parameter optimization techniques. In the experiments, the proposed IDS has demonstrated over 99.25% detection rates and F1-scores on two well-known public benchmark IoV security datasets: the Car-Hacking dataset and the CICIDS2017 dataset. This shows the effectiveness of the proposed IDS for cyber-attack detection in both intra-vehicle and external vehicular networks.

<p float="left">
  <img src="https://github.com/Western-OC2-Lab/Intrusion-Detection-System-Using-CNN-and-Transfer-Learning/blob/main/framework.png" width="500" />
  <img src="https://github.com/Western-OC2-Lab/Intrusion-Detection-System-Using-CNN-and-Transfer-Learning/blob/main/CAN.png" width="400" /> 
</p>

## Implementation 
### CNN Models  
* VGG16
* VGG19
* Xception
* Inception
* Resnet
* InceptionResnet

### Ensemble Learning Models
* Bagging
* Probability Averaging
* Concatenation

### Hyperparameter Optimization Methods
* Random Search (RS)
* Bayesian Optimization - Tree Parzen Estimator(BO-TPE)

### Dataset 
1. CAN-intrusion/Car-Hacking dataset, a benchmark network security dataset for intra-vehicle intrusion detection
* Publicly available at: https://ocslab.hksecurity.net/Datasets/CAN-intrusion-dataset  
* Can be processed using the same code

2. CICIDS2017 dataset, a popular network traffic dataset for intrusion detection problems
* Publicly available at: https://www.unb.ca/cic/datasets/ids-2017.html  

For the purpose of displaying the experimental results in Jupyter Notebook, the sampled subset of the CAN-intrusion dataset is used in the sample code. The subsets are in the "[data](https://github.com/Western-OC2-Lab/Intrusion-Detection-System-Using-CNN-and-Transfer-Learning/tree/main/data)" folder.

### Code  
* [1-Data_pre-processing_CAN.ipynb](https://github.com/Western-OC2-Lab/Intrusion-Detection-System-Using-CNN-and-Transfer-Learning/blob/main/1-Data_pre-processing_CAN.ipynb): code for data pre-processing and transformation (tabular data to images).  
* [2-CNN_Model_Development&Hyperparameter Optimization.ipynb](https://github.com/Western-OC2-Lab/Intrusion-Detection-System-Using-CNN-and-Transfer-Learning/blob/main/2-CNN_Model_Development%26Hyperparameter%20Optimization.ipynb): code for the development and CNN models and their hyperparameter optimization.
* [3-Ensemble_Models-CAN.ipynb](https://github.com/Western-OC2-Lab/Intrusion-Detection-System-Using-CNN-and-Transfer-Learning/blob/main/3-Ensemble_Models-CAN.ipynb): code for the construction of three ensemble learning techniques.

Libraries  
* Python 3.5+
* [Keras 2.1.0+](hhttps://keras.io/)  
* [Tensorflow 1.10.0+](https://www.tensorflow.org/install/gpu)
* [OpenCV-python](https://docs.opencv.org/4.x/d6/d00/tutorial_py_root.html)
* [hyperopt](https://github.com/hyperopt/hyperopt) 

## Contact-Info
Please feel free to contact us for any questions or cooperation opportunities. We will be happy to help.
* Email: [liyanghart@gmail.com](mailto:liyanghart@gmail.com) or [Abdallah.Shami@uwo.ca](mailto:Abdallah.Shami@uwo.ca)
* GitHub: [LiYangHart](https://github.com/LiYangHart) and [Western OC2 Lab](https://github.com/Western-OC2-Lab/)
* LinkedIn: [Li Yang](https://www.linkedin.com/in/li-yang-phd-65a190176/)  
* Google Scholar: [Li Yang](https://scholar.google.com.eg/citations?user=XEfM7bIAAAAJ&hl=en) and [OC2 Lab](https://scholar.google.com.eg/citations?user=oiebNboAAAAJ&hl=en)

## Citation
If you find this repository useful in your research, please cite this article as:  

L. Yang and A. Shami, "A Transfer Learning and Optimized CNN Based Intrusion Detection System for Internet of Vehicles," ICC 2022 - IEEE International Conference on Communications, 2022, pp. 2774-2779, doi: 10.1109/ICC45855.2022.9838780.

```
@INPROCEEDINGS{9838780,
  author={Yang, Li and Shami, Abdallah},
  booktitle={ICC 2022 - IEEE International Conference on Communications}, 
  title={A Transfer Learning and Optimized CNN Based Intrusion Detection System for Internet of Vehicles}, 
  year={2022},
  pages={2774-2779},
  doi={10.1109/ICC45855.2022.9838780}}
```
