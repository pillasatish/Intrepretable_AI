# Interpretable AI For Protein Expression Images and Associated Clinical Metadata

## 1. Introduction

With a conservative frequency estimate of about 1:5,000, mitochondrial disorders are among the most prevalent inheritable diseases [1]. Diagnosis and understanding of the different mitochondrial diseases are extremely difficult because they have a wide range of symptoms in each patient and affect different organs and tissues of the body [2]. However, recent studies show deep learning algorithms with interpretability and explainability, especially Convolutional Neural Networks (CNN), can help us automatically diagnose and evaluate different diseases by detecting the different patterns in the images. In the study, we developed deep learning models using transfer learning to predict mitochondrial diseases and used existing machine learning interpretability and explainability AI approaches for computer vision, like Grad-CAM [3], and Neural Disentanglement (concept whitening) [4], to understand the features that result in the prediction of mitochondrial disease from protein expression images.

## 2. Aim

To determine if Deep Learning (DL) can be used as a reliable method to classify mitochondrial diseases using interpretability
and explainability approaches.

• Interpretability Method: Neural Disentanglement

• Explainability Method: Saliency Map 

## 3. Objective

This investigation has primarily two objectives:

3.1. Determine whether it is possible to accurately diagnose mitochondrial diseases.

>  Adapt the pre-trained deep learning models like VGG16 and ResNet-50 to classify different mitochondrial diseases using protein expression images obtained by image mass cytometry.     Evaluate, compare, and fine-tune different pre-trained model architectures using parameters like accuracy, precision, recall, f1 score, and confusion matrix.

3.2. Understand the underlying pathology of mitochondrial diseases.

> Once we know that the pre-trained deep learning models are able to classify different mitochondrial diseases, we can make then apply different interpretability and explainability AI approaches such as Grad-CAM and Neural Disentanglement on top of the pre-train models to understand the underlying pathology of mitochondrial diseases. 

## 4. Steps to execute this Project.

1. Download/fork/clone the project by clicking [here](https://github.com/pillasatish/Intrepretable_AI).

2. Once the repository is downloaded one can see that the folder contains four sub-folders and a readme file. Each sub-folder is named according to the research work undertaken during the thesis.  

3. The first folder Concept Whitening contains one ipynb file (Concept_Whitening.ipynb) and 5 py files:
	a. Plot_function.py: to plot the required graph

	b. train_isis.py: To train the model

	c. resnet18365.py: To build the initial resent 18 model

	d. iterative_normaliztion: contains code to implement concept whitening

	e. model_resent.py: to build the concept whitening resnet model.

4. The Second folder Multi-channel Stacked protein Images contains one ipynb file (Multi-channel_VGG16.ipynb).

5. The third folder Single Channel Protein Images(SDHA) contains two ipynb files (Grad-CAM_VGG16 and Grad-CAM_ResNet-50).

6. Download/fork/clone the dataset by clicking [here](https://github.com/atifkhanncl/interpretable_AI).

7. Once the dataset is downloaded zip it and upload the dataset to google drive. 

8. One can run an experiment related to Single Channel Protein Images(SDHA) or multi-channel stack protein images analysis by just uploading the notebook related to the experiment they belong to. For example, if one wants to check the Grad-CAM results they can upload the GRAD-CAM_VGG16.ipynb or GRAD-CAM_ResNet-50.ipynb file to google colab and run all the cells to check the results. One must ensure to change the unzip dataset path in the google colab notebook as per where they have uploaded the dataset. The remaining steps are automated, one just needs to run all the cells for reproducibility.

9. For concept whitening first we need to open google colab and upload the Concept_whitening_pytorch.ipynb file. In addition to that, there are 5 (.py files) which need to be uploaded to the session storage when the session is started. Once the two steps are completed one just needs to run all the cells for easy reproducibility.
 

## 5. Reports

The last sub-folder is the report folder contains files related main report, presentation, and poster in pdf format:

1. Main report generated by rmarkdown: This file contains all the analysis, methods, results, and conclusions of the research work undertaken. This file is in ./reports/B210472095_CSC8639_Thesis.pdf.

2. Presentation file: This file contains the presentation slide related to the research work undertaken. This file is in ./reports/B210472095_CSC8639_Presentation.pdf.

3. Poster file: This file contains a summary of the research in poster format. This file is in ./reports/This file is in ./reports/B210472095_CSC8639_Poster.pdf.

## 6. Reference

1. Gorman, A. M. Schaefer, Y. Ng, N. Gomez, and Blakely, “Prevalence of nuclear and mitochondrial DNA mutations related to adult mitochondrial disease,” Annals of Neurology, vol. 77. Wiley Online Library, pp. 753–759, 2015.

2. P. Forny, E. Footitt, J. E. Davison, A. Lam, and Woodward, “Diagnosing mitochondrial disorders remains challenging in the omics era,” Neurology. Genetics, vol. 7. p. e597, 2021. doi:10.1212/NXG.0000000000000597.

3. LR. R. Selvaraju, M. Cogswell, A. Das, R. Vedantam, D. Parikh, and D. Batra, “GradCAM: Visualexplanations from deep networks via gradient-based localization,” International journal of computer vision, vol. 128. pp. 336–359, 2020. doi: 10.1007/s11263-019-01228-7.

4. Z. Chen, Y. Bei, and C. Rudin, “Concept whitening for interpretable image recognition,” NatureMachine Intelligence, vol. 2, no. 12, pp. 772–782, 2020, doi: 10.1038/s42256-02000265-z.
