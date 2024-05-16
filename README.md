# CIFAR10-ImageClassfication 🖼️
An Image Classification project w/ MobileNetV2 and DenseNet-121. Leveraging techniques like Hyperparameter Tuning, Transfer Learning, Imagine Preprocessing Techniques and Ensemble Methods. 

Overview of entire project: [CIFAR-10 Image Classificaiton Presentation](https://www.canva.com/design/DAGDyqFWRIY/RAk4XL0xich_XI2wHAAWOg/edit?utm_content=DAGDyqFWRIY&utm_campaign=designshare&utm_medium=link2&utm_source=sharebutton)

View the Full Report here: [Full Report](https://docs.google.com/document/d/1GTMfviF-TvSTIBa5T1_in5LMp3R-I0pt0QUzbbgMQYE/edit?usp=drive_link)

Full project at: [Full Source Codes (1.0 to 3.2)](https://drive.google.com/drive/folders/1OLIl8K3Bo1wY9SUzBPyOX-0uuSmyeMsk?usp=sharing)

Ablation Study:<br>
7 iteration of MobileV2 Settings 📱: 

| Enhancements Approaches     | 1.0 | 1.1 | 2.0 | 2.1 | 2.2 | 2.3 | 2.4 |
|-----------------------------|-----|-----|-----|-----|-----|-----|-----|
| Increasing Epochs           | ✔   | ✔   |     | ✔   | ✔   |     | ✔   |
| Bicubic Interpolation       |     | ✔   |     |     | ✔   |     |     |
| Random Rotation             |     |     |     |     |     |     |     |
| Gaussian Blur               | ✔   |     |     |     |     |     |     |
| Transfer Learning           |     |     |     |     |     |     |     |
| Decreased Learning Rate     |     |     | ✔   |     |     | ✔   |     |
| Increased Batch Size        |     |     |     | ✔   |     | ✔   | ✔   |
| AdamW Optimization          |     |     |     |     | ✔   |     | ✔   |
| Weighted Class Training     |     |     |     |     |     | ✔   |     |

2 iteration of DenseNet-121 Settings:
| Enhancements Approaches   | 3.0 | 3.1 |
|---------------------------|-----|-----|
| Increase Epochs           | ✔   | ✔   |
| Increase Batch Size       | ✔   | ✔   |
| Weighted Class Training   | ✔   | ✔   |
| Transfer Learning         |     | ✔   |
| Decreased Learning Rate   |     | ✔   |

Ensemble Results using Soft Voting (2.4 + 3.2) : 
| Model  | F1-Scores |      |          | Accuracy |      |          |
|--------|-----------|------|----------|----------|------|----------|
|        | Train     | Test | Improvement | Train  | Test | Improvement |
| **2.4**  | 0.9442    | 0.8874 | -        | 0.9430 | 0.8842 | -        |
| **3.1**  | 0.9802    | 0.9235 | +0.0361   | 0.9802 | 0.9234 | +0.0392   |
| **3.2 (2.4+3.1)** | 0.9859    | 0.9342 | +0.0107   | 0.9859 | 0.9341 | +0.0107   |

![image](https://github.com/Bernardbyy/CIFAR10-ImageClassfication/assets/75737130/ed26d623-23d9-4506-ba3f-7826060f1096)


