# GAViD: A Large-Scale Multimodal Dataset for Context-Aware Group Affect Recognition from Videos
Implementation for the paper submitted to ACM Multimedia Conference (ACMMM) 2025.

# 🔍💡 Abstract
Recognizing group affect in in-the-wild settings remains challenging due to two key factors: the difficulty of capturing and labeling group data and the complexity of analyzing group affect amid diverse interactions and contextual variability. The lack of comprehensive datasets annotated with multimodal and contextual information further limits advances in the field. To address this, we introduce the Group Affect from ViDeos (GAViD) dataset, comprising 5091 video clips with multimodal data (video, audio and context), annotated with ternary valence and discrete emotion labels and enriched with VideoGPT-generated contextual metadata and human-annotated action cues. We also present CAGNet, a baseline model for multimodal context-aware group affect recognition. CAGNet achieves 61.20% test accuracy on GAViD, comparable to state-of-the-art performance.
---

# 📄 Code Files
The code files are currently private and will be made public after the acceptance/publication of the corresponding paper.
---
# ✏️ Dataset Details & Access
The IIT Roorkee Multimodal Video based Affect recognition (GAViD) Dataset has been compiled by Deepak Kumar, Abhsihsek Singh at Machine Vision Lab, IIT Roorkee under the supervision of Prof. Balasubramanian Raman. It Consists of 5091 video clips. The data is colleted from the youtube under the creative comman license policy.

## Compliance with Facebook's Terms & Conditions
The data (videos) has been collected manually from YouTube with keywords such as Protest, Wedding Dance, Group Meeting etc. 
---
# 🔄📋🪜 Steps Involved in the Dataset Compilation Process
Below are the steps involved in the dataset compilation process.

**Step 1: Manual search of video with CC licence from the youtube**
1. Videos were sourced from YouTube under the Creative Commons CC BY license,following the ethical protocols.
2. Included only videos that were CC-licensed and featured two or more individuals to capture real-world group dynamics.

**Step 2: Segmenting the Videos in the clips of 5 Secs**
1. All videos were split into 5-second clips using FFmpeg.
2. Retained up to 35 segments per source video, covering the majority of group members despite dynamic framing.

**Step 3: Data Preprocessing**
1. All segmented clips underwent a manual verification process.
2. Clips were excluded if they lacked a discernible group structure, such as the presence of a complete or partial group, or if the faces of all visible group members were not clearly detectable, which could compromise annotation accuracy

**Step 3: Manual Annotation of video clips**
- Used Labelbox for annotation.
- Clips were placed into 100 bins and assigned to 108 annotators (60 male, 48 female; average age 28 ± 5 years).
- Three annotators viewed each clip and labeled group emotion (positive, neutral, negative), discrete emotion (happy, sad, fear, anger, neutral), intensity (high, medium, low), interaction type (cooperative, hostile, neutral) and action cues (e.g. smiling, clapping, shouting, dancing, singing, fighting, conversation, heated debate, protest, team activity).
- The final label was decided by majority vote.
---
# 📝 Dataset Description
Below table is representing the dataset details. Here, ‘P’: Positive, ‘N’: Negative, ‘Ne’: Neutral, ‘H’: Happy, ‘S’: Sad, ‘F’: Fear, ‘A’: Anger.

![Alt Text](/Dataset_Details.png)
---
# 🏷️ ➜ ⚙️ ➜ 🤖 Dataset Annotation Process Pipeline
### Overview of the GAViD annotation pipeline and interface. The diagram illustrates stages of data collection, sample video frames with valence, emotion, intensity, cues and contextual labels, as well as the Labelbox interface used for multi-annotator input. Sample context descriptions and [VideoGPT](https://github.com/mbzuai-oryx/Video-ChatGPT)-suggested keywords demonstrate how human and AI annotations are integrated.
![Alt Text](/fig_DataCompilation.png)
---
# 🧩🛠️ Data Annotation tool used
We have used [labelbox](https://labelbox.com/) for the annotation.

Below is the iamge for one sample used in the annotation
![Alt Text](/labelbox.png)
---
# 🏗️🧱 CAGNet Architecture Diagram
We propose CAGNet, a baseline GAR model that fuses visual, audio and contextual information tas shown in the diagram.
![Alt_Text](/fig_CAGNet.png)
---
# 📦 Dataset Availability
### Access to the IIT-R GAViD dataset can be obtained by zenodo link: https://zenodo.org/records/15448846
#### NOTE: For now we are providing only Train video clips. The corresponding paper is under Review in ACM Multimedia 2025 Dataset Track. After its publication, the validation and Test set access will be granted upon request and approval, in accordance with the Responsible Use Policy.
