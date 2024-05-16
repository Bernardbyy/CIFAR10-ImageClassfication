# CIFAR10-ImageClassfication
An Image Classification project w/ MobileNetV2 and DenseNet-121. Leveraging techniques like Hyperparameter Tuning, Transfer Learning, Imagine Preprocessing Techniques and Ensemble Methods. 

Overview of entire project: https://www.canva.com/design/DAGDyqFWRIY/RAk4XL0xich_XI2wHAAWOg/edit?utm_content=DAGDyqFWRIY&utm_campaign=designshare&utm_medium=link2&utm_source=sharebutton

View the Full Report here: https://docs.google.com/document/d/1GTMfviF-TvSTIBa5T1_in5LMp3R-I0pt0QUzbbgMQYE/edit?usp=drive_link

Full project at: https://drive.google.com/drive/folders/1OLIl8K3Bo1wY9SUzBPyOX-0uuSmyeMsk?usp=sharing

Ablation Study: 
Settings: 

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

<table>
    <thead>
        <tr>
            <th>Enhancements Approaches</th>
            <th>1.0</th>
            <th>1.1</th>
            <th>2.0</th>
            <th>2.1</th>
            <th>2.2</th>
            <th>2.3</th>
            <th>2.4</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td>Increasing Epochs</td>
            <td>✔</td>
            <td>✔</td>
            <td></td>
            <td>✔</td>
            <td>✔</td>
            <td></td>
            <td>✔</td>
        </tr>
        <tr>
            <td>Bicubic Interpolation</td>
            <td></td>
            <td>✔</td>
            <td></td>
            <td></td>
            <td>✔</td>
            <td></td>
            <td></td>
        </tr>
        <tr>
            <td>Random Rotation</td>
            <td></td>
            <td></td>
            <td></td>
            <td></td>
            <td></td>
            <td></td>
            <td></td>
        </tr>
        <tr>
            <td>Gaussian Blur</td>
            <td>✔</td>
            <td></td>
            <td></td>
            <td></td>
            <td></td>
            <td></td>
            <td></td>
        </tr>
        <tr>
            <td>Transfer Learning</td>
            <td></td>
            <td></td>
            <td></td>
            <td></td>
            <td></td>
            <td></td>
            <td></td>
        </tr>
        <tr>
            <td>Decreased Learning Rate</td>
            <td></td>
            <td></td>
            <td>✔</td>
            <td></td>
            <td></td>
            <td>✔</td>
            <td></td>
        </tr>
        <tr>
            <td>Increased Batch Size</td>
            <td></td>
            <td></td>
            <td></td>
            <td>✔</td>
            <td></td>
            <td>✔</td>
            <td>✔</td>
        </tr>
        <tr>
            <td>AdamW Optimization</td>
            <td></td>
            <td></td>
            <td></td>
            <td></td>
            <td>✔</td>
            <td></td>
            <td>✔</td>
        </tr>
        <tr>
            <td>Weighted Class Training</td>
            <td></td>
            <td></td>
            <td></td>
            <td></td>
            <td></td>
            <td>✔</td>
            <td></td>
        </tr>
    </tbody>
</table>
