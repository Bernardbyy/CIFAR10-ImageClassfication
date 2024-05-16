# CIFAR10-ImageClassfication 🖼️

An Image Classification project utilizing MobileNetV2 and DenseNet-121. This project leverages advanced techniques to enhance model performance and accuracy, including:

| Index | Technique                    | Description                                               | Specific Details                                 |
|-------|------------------------------|-----------------------------------------------------------|--------------------------------------------------|
| 1     | Cross Validation             | Utilized to ensure that the model generalizes well to new data. | 5-fold cross-validation applied.                 |
| 2     | Early Stopping               | To prevent overfitting by stopping training when validation metrics stop improving. | Patience level set to 5 epochs.                  |
| 3     | Transfer Learning            | Applying knowledge gained from one problem to a different but related problem. | Leveraging pre-trained weights.                  |
| 4     | Hyperparameter Tuning        | Systematically searching for the optimal parameters of a model. | Tuning epoch, batch size, and learning rate.     |
| 5     | Data Augmentation            | Increasing the diversity of data available for training models without actually collecting new data. | Includes random rotation, Gaussian blur, resizing, and bicubic interpolation. |
| 6     | Changing Optimization Algorithms | Experimenting with different optimizers to improve training performance. | Switch from Adam to AdamW optimizer.             |
| 7     | Weighted Class Training      | Adjusting the importance of a class based on its weight to address class imbalance. | More emphasis on classes like cats, dogs, birds, and planes. |
| 8     | Ensemble Methods             | Combining predictions from multiple models to improve accuracy. | Soft voting ensemble of MobileNetV2 and DenseNet-121 logits. |

This table provides an at-a-glance overview of the methodologies and specific adaptations made to optimize the CIFAR10 Image Classification project.


Overview of entire project: [CIFAR-10 Image Classification Presentation](https://www.canva.com/design/DAGDyqFWRIY/RAk4XL0xich_XI2wHAAWOg/edit?utm_content=DAGDyqFWRIY&utm_campaign=designshare&utm_medium=link2&utm_source=sharebutton)

View the Full Report here: [Full Report](https://docs.google.com/document/d/1GTMfviF-TvSTIBa5T1_in5LMp3R-I0pt0QUzbbgMQYE/edit?usp=drive_link)

Full project at: [Full Source Codes (1.0 to 3.2)](https://drive.google.com/drive/folders/1OLIl8K3Bo1wY9SUzBPyOX-0uuSmyeMsk?usp=sharing)

Ablation Study:<br>
7 iteration of MobileV2 Settings 📱: 

| Enhancements Approaches     | 1.0 | 1.1 | 2.0 | 2.1 | 2.2 | 2.3 | 2.4 |
|-----------------------------|-----|-----|-----|-----|-----|-----|-----|
| Increasing Epochs           | ✔   | ✔   | ✔  | ✔   | ✔   |  ✔   | ✔   |
| Bicubic Interpolation       |     | ✔   | ✔  | ✔   | ✔   |  ✔   |    ✔ |
| Random Rotation             |     | ✔   |     |     |     |     |     |
| Gaussian Blur               |     | ✔   |     |     |     |     |     |
| Transfer Learning           |     |     | ✔   |✔   |  ✔   |  ✔   |  ✔   |
| Decreased Learning Rate     |     |     |     | ✔   |  ✔   | ✔   |  ✔   |
| Increased Batch Size        |     |     |     |     |  ✔   | ✔   | ✔   |
| AdamW Optimization          |     |     |     |     |    |   ✔  | ✔   |
| Weighted Class Training     |     |     |     |     |     |    |    ✔ |

2 iteration of DenseNet-121 Settings:
| Enhancements Approaches   | 3.0 | 3.1 |
|---------------------------|-----|-----|
| Increase Epochs           | ✔   | ✔   |
| Increase Batch Size       | ✔   | ✔   |
| Weighted Class Training   | ✔   | ✔   |
| Transfer Learning         |     | ✔   |
| Decreased Learning Rate   |     | ✔   |

Ensemble Results using Soft Voting (2.4 + 3.1) : 
| Model  | F1-Scores |      |          | Accuracy |      |          |
|--------|-----------|------|----------|----------|------|----------|
|        | Train     | Test | Improvement | Train  | Test | Improvement |
| **2.4**  | 0.9442    | 0.8874 | -        | 0.9430 | 0.8842 | -        |
| **3.1**  | 0.9802    | 0.9235 | +0.0361   | 0.9802 | 0.9234 | +0.0392   |
| **3.2 (2.4+3.1)** | 0.9859    | 0.9342 | +0.0107   | 0.9859 | 0.9341 | +0.0107   |

Ensemble Method Results across individual classes : <br>
F1-Score: 
![image](https://github.com/Bernardbyy/CIFAR10-ImageClassfication/assets/75737130/383575bd-5870-468f-82f8-d3e2acc8976e)

Precision: 
![image](https://github.com/Bernardbyy/CIFAR10-ImageClassfication/assets/75737130/ed26d623-23d9-4506-ba3f-7826060f1096)

Recall: 
![image](https://github.com/Bernardbyy/CIFAR10-ImageClassfication/assets/75737130/c4e5aff6-41b3-4d1a-8b3e-1e9e6ff2002c)


