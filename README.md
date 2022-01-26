# Intrusion-Detection-System-Using-CNN-and-Transfer-Learning

This is the code for the paper entitled "**[A Transfer Learning and Optimized CNN Based Intrusion Detection System for Internet of Vehicles](https://arxiv.org/pdf/2109.05013.pdf)**" accepted in **IEEE International Conference on Communications (IEEE ICC)**.  
Authors: Li Yang and Abdallah Shami  
Organization: The Optimized Computing and Communications (OC2) Lab, ECE Department, Western University

This repository also introduces **concept drift definitions** and **online machine learning methods** for **data stream analytics** using the **[River](https://riverml.xyz/dev/)** library.  
Another **tutorial code** for **concept drift, online machine learning, and data stream analytics** can be found in: [OASW-Concept-Drift-Detection-and-Adaptation](https://github.com/Western-OC2-Lab/OASW-Concept-Drift-Detection-and-Adaptation)



## Abstract of The Paper
As the number of Internet of Things (IoT) devices and systems have surged, IoT data analytics techniques have been developed to detect malicious cyber-attacks and secure IoT systems; however, concept drift issues often occur in IoT data analytics, as IoT data is often dynamic data streams that change over time, causing model degradation and attack detection failure. This is because traditional data analytics models are static models that cannot adapt to data distribution changes. In this paper, we propose a Performance Weighted Probability Averaging Ensemble (PWPAE) framework for drift adaptive IoT anomaly detection through IoT data stream analytics. Experiments on two public datasets show the effectiveness of our proposed PWPAE method compared against state-of-the-art methods.

## Implementation 
### Online Learning/Concept Drift Adaptation Algorithms  
* Adaptive Random Forest (ARF)
* Streaming Random Patches (SRP)
* Extremely Fast Decision Tree (EFDT)
* Hoeffding Tree (HT)
* Leveraging Bagging (LB)
* Performance Weighted Probability Averaging Ensemble (PWPAE)
  * Proposed Method

### Drift Detection Algorithms
* Adaptive Windowing (ADWIN)
* Drift Detection Method (DDM)

### Dataset 
1. IoTID20 dataset, a novel IoT botnet dataset
   * Publicly available at: https://sites.google.com/view/iot-network-intrusion-dataset/home

2. CICIDS2017 dataset, a popular network traffic dataset for intrusion detection problems
   * Publicly available at: https://www.unb.ca/cic/datasets/ids-2017.html  

For the purpose of displaying the experimental results in Jupyter Notebook, the sampled subsets of the two datasets are used in the sample code. The subsets are in the "[data](https://github.com/Western-OC2-Lab/PWPAE-Concept-Drift-Detection-and-Adaptation/tree/main/data)" folder.

### Code  
* [globecom2021_PWPAE_IoTID20.ipynb](https://github.com/Western-OC2-Lab/PWPAE-Concept-Drift-Detection-and-Adaptation/blob/main/globecom2021_PWPAE_IoTID20.ipynb): code for the sampled IoTID20 dataset.  
* [globecom2021_PWPAE_CICIDS2017.ipynb](https://github.com/Western-OC2-Lab/PWPAE-Concept-Drift-Detection-and-Adaptation/blob/main/globecom2021_PWPAE_CICIDS2017.ipynb): code for the sampled CICIDS2017 dataset.

### Requirements & Libraries  
* Python 3.5+
* [Keras 2.1.0](https://scikit-learn.org/stable/)  
* [Tensorflow 1.10.0](https://lightgbm.readthedocs.io/en/latest/)

## Contact-Info
Please feel free to contact us for any questions or cooperation opportunities. We will be happy to help.
* Email: [liyanghart@gmail.com](mailto:liyanghart@gmail.com) or [Abdallah.Shami@uwo.ca](mailto:Abdallah.Shami@uwo.ca)
* GitHub: [LiYangHart](https://github.com/LiYangHart) and [Western OC2 Lab](https://github.com/Western-OC2-Lab/)
* LinkedIn: [Li Yang](https://www.linkedin.com/in/li-yang-65a190176/)  
* Google Scholar: [Li Yang](https://scholar.google.com.eg/citations?user=XEfM7bIAAAAJ&hl=en) and [OC2 Lab](https://scholar.google.com.eg/citations?user=oiebNboAAAAJ&hl=en)

## Citation
If you find this repository useful in your research, please cite this article as:  

L. Yang and A. Shami, "A Transfer Learning and Optimized CNN Based Intrusion Detection System for Internet of Vehicles," in 2022 IEEE International Conference on Communications (ICC), Seoul, South Korea, 2022, pp. 1-6.

```
@INPROCEEDINGS{1570723427,
  author={Yang, Li and Shami, Abdallah},
  booktitle={2022 IEEE International Conference on Communications (ICC)}, 
  title={A Transfer Learning and Optimized CNN Based Intrusion Detection System for Internet of Vehicles,}, 
  year={2022},
  pages={1-6},
  doi={}
  }
```
