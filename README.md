# GAViD
This is the repository for the GAViD: Group Affect from ViDeos Dataset

# Abstract
Recognizing group affect in in-the-wild settings remains challenging due to two key factors: the difficulty of capturing and labeling group data and the complexity of analyzing group affect amid diverse interactions and contextual variability. The lack of comprehensive datasets annotated with multimodal and contextual information further limits advances in the field. To address this, we introduce the Group Affect from ViDeos (GAViD) dataset, comprising 5091 video clips with multimodal data (video, audio and context), annotated with ternary valence and discrete emotion labels and enriched with VideoGPT-generated contextual metadata and human-annotated action cues. We also present CAGNet, a baseline model for multimodal context-aware group affect recognition. CAGNet achieves 61.20% test accuracy on GAViD, comparable to state-of-the-art performance.




# Code Files
The code files are currently private and will be made public after the acceptance/publication of the corresponding paper.

# Dataset Details & Access
The IIT Roorkee Multimodal Video based Affect recognition (GAViD) Dataset has been compiled by Deepak Kumar, Abhsihsek Singh at Machine Vision Lab, IIT Roorkee under the supervision of Prof. Balasubramanian Raman. It Consists of 5091 video clips. The data is colleted from the youtube under the creative comman licence policy.

## Compliance with Facebook's Terms & Conditions
ggg

# Steps Involved in the Data Collection
gggg

**Step 1: Manual search of video with CC licence from the youtube**
1. sss

**Step 2: Segmenting the Videos in the clips of 5 Secs**
1. hkjhkhk
2. kkkk
   
**Step 3: Manual Annotation of vidoe clips**
- ss
- rr

# Dataset Description
Below table is representing the dataset details. Here, ‘P’: Positive, ‘N’: Negative, ‘Ne’: Neutral, ‘H’: Happy, ‘S’: Sad, ‘F’: Fear, ‘A’: Anger.
![Alt Text](/Dataset_Details.png)

# Dataset Annotation Process Pipeline
### Overview of the GAViD annotation pipeline and interface. The diagram illustrates stages of data collection, sample video frames with valence, emotion, intensity, cues and contextual labels, as well as the Labelbox interface used for multi-annotator input. Sample context descriptions and [VideoGPT](https://github.com/mbzuai-oryx/Video-ChatGPT)-suggested keywords demonstrate how human and AI annotations are integrated.
![Alt Text](/fig_DataCompilation.png)

# Data Annotation tool used
We have used [labelbox](https://labelbox.com/) for the annotation.

Below is the iamge for one sample used in the annotation
![Alt Text](/labelbox.png)

# CAGNet Architecture Diagram
We propose CAGNet, a baseline GAR model that fuses visual, audio and contextual information tas shown in the diagram.
![Alt_Text](/fig_CAGNet.png)

Access to the IIT-R GAViD dataset can be obtained by through: https://zenodo.org/records/15448846

