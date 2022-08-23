# Pneumonia Detection using the InceptionV3 Network

## About

<p>The dataset is organized into 3 folders (train, test, val) and contains subfolders for each image category (Pneumonia/Normal). There are 5,863 X-Ray images (JPEG) and 2 categories (Pneumonia/Normal).</p>

<p>Chest X-ray images (anterior-posterior) were selected from retrospective cohorts of pediatric patients of one to five years old from Guangzhou Women and Children’s Medical Center, Guangzhou. All chest X-ray imaging was performed as part of patients’ routine clinical care.</p>

<p>For the analysis of chest x-ray images, all chest radiographs were initially screened for quality control by removing all low quality or unreadable scans. The diagnoses for the images were then graded by two expert physicians before being cleared for training the AI system. In order to account for any grading errors, the evaluation set was also checked by a third expert.</p>

## Dataset

<p>The for the network used dataset was downloaded from <a href="https://www.kaggle.com/paultimothymooney/chest-xray-pneumonia">Kaggle</a>
<p>The original dataset can be found <a href="https://data.mendeley.com/datasets/rscbjbr9sj/2">here</a>

## Local Installation

### Clone the repo (or simply download it)
```shell
git clone https://github.com/JanMarcelKezmann/Pneumonia-Detection-InceptionV3-Transfer-Learning.git
```

### Install requirements
##### (go into the new folder)

```shell
pip install -r requirements.txt
```

### Run with JupyterNotebook or JupyterLab
<p>Just open the .ipynb code in a Notebook of your choice and run it.</p>

## Results

<p>Training the model with a on the imagenet dataset pretrained InceptionV3 model gives the follwing scores:</p>

- Accuracy: 0.7131
- F1 Score: 0.7954
- Precision Score: 0.7175
- Recall Score: 0.8923

<p>We get a lot better results if we use only the untrained InceptionV3 as a base model and train all of it.</p>
<p>Here we got the following results:</p>

- Accuracy: 0.8413
- F1 Score: 0.8871
- Precision Score: 0.7988
- Recall Score: 0.9974

<p align="center">
  <img src="https://user-images.githubusercontent.com/50111329/65390868-b1247200-dd62-11e9-93cb-f2f1bc0788c3.png" width="800px" alt="">
</p>

<p>The Confusion Matrix of the Second Model</p>
<p align="left">
  <img src="https://user-images.githubusercontent.com/50111329/65390959-a1f1f400-dd63-11e9-868c-0e8c52a1d4b7.png" width="400px" alt="">
</p>

## Acknowledgements
<p>My work was partially inspired by <a href="https://www.kaggle.com/aakashnain/beating-everything-with-depthwise-convolution">this</a> Kaggle Kernel and <a href="">this</a> Github Repository.</p>

## Support, Questions or Bugs
<p>Just write me an E-Mail: j-m.kezmann@t-online.de</p>
<p>Or contact we via <a class="facebook" href="https://www.facebook.com/janmarcel.kezmann">facebook</a>.</p>
