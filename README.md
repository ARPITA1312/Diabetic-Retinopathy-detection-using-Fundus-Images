# Diabetic-Retinopathy-detection-using-Fundus-Images
Quantum Transfer Learning for Enhanced Diabetic Retinopathy Detection with U-Net Segmentation of Fundus Images 
Abstract: Diabetic Retinopathy (DR) is one of the leading causes of blindness, particularly among diabetic patients, as it introduces numerous lesions to the retina. Traditional identification of DR through the analysis of retinal fundus images by ophthalmologists is a time-consuming and costly process. Despite the effectiveness of classical transfer learning models in Computer-Aided Diagnosis for DR detection, they face significant challenges, including high training costs, computational complexity, and resource intensity.
![image](https://github.com/user-attachments/assets/ac79782a-1e54-4242-beb4-461c3dd31aa7)
This research proposes a Quantum Transfer Learning (QTL) methodology integrated with classical machine learning models for quantitative and qualitative improvements in DR detection. Using the APTOS 2019 Blindness Detection dataset, we leverage pre-trained models such as ResNet-18, ResNet-34, ResNet-50, ResNet-101, and ResNet-152, alongside Inception V3 for feature extraction. Our method employs a Variational Quantum Classifier, achieving an accuracy of 97% with the ResNet-18 model. Furthermore, the U-Net model is used for DR stage segmentation, achieving a testing accuracy of 96.94% on the STARE dataset. To enhance classification results, Support Vector Machine (SVM) and K Nearest Neighbour (KNN) models were also utilized, achieving accuracies above 96.62%. This quantum-classical approach demonstrates that QTL enhances DR detection, providing faster and more accurate diagnoses for diabetic retinopathy patients.

👁️ What is Diabetic Retinopathy? Diabetic Retinopathy is a condition that can lead to vision loss and blindness in individuals with diabetes. It affects the blood vessels in the retina and is one of the leading causes of blindness globally. Early detection is crucial, as it can help patients take preventive measures to protect their vision.

🚀 Problem Statement The objective of this project is to perform image classification on fundus photographs, predicting which class the given image belongs to. The classes are:

0 - Normal 1 - Mild 2 - Moderate 3 - Severe 4 - Proliferative

🛠️ Proposed Methodology
We utilize the ResNet model for classifying images, built using PyTorch. The ResNet architecture consists of 152 layers, addressing the vanishing gradient problem through skip connections. This allows us to train ultra-deep networks effectively while maintaining high accuracy on large datasets.

In addition to ResNet, the U-Net model is employed for segmenting retinal lesions associated with diabetic retinopathy. U-Net is a convolutional neural network architecture designed specifically for image segmentation tasks. It features an encoder-decoder structure with skip connections that help retain spatial information lost during down-sampling. This model excels in capturing fine details, making it ideal for detecting and localizing lesions in fundus images.

The dataset comprises 3662 training images and approximately 1900 testing images. Additionally, a GUI developed using Tkinter enables users to upload fundus retinal images and receive predicted labels as output.
Architecture
The ResNet model employs skip connections that facilitate the training of deep networks without encountering vanishing gradient issues. Instead of learning the underlying mapping 𝐻(𝑥), the network fits the residual mapping 𝐹(𝑥). This architecture enhances the model's performance significantly.

The U-Net model consists of an encoder path for down-sampling and a decoder path for up-sampling, allowing it to generate high-resolution segmentations from low-resolution inputs. The skip connections between the encoder and decoder paths retain critical features, enabling precise localization of retinal lesions.

🖼 U-Net Model for Segmentation The U-Net model is employed for DR stage segmentation, which excels in biomedical image segmentation tasks. It utilizes an encoder-decoder architecture to capture context and precise localization. This model significantly contributes to effective segmentation of retinal lesions, aiding in better classification.

⚙️ Technologies Used Framework: PyTorch Models: ResNet-18, ResNet-34, ResNet-50, ResNet-101, ResNet-152, Inception V3, U-Net Datasets: APTOS 2019 Blindness Detection, STARE

🌍 Area of Applications The classification of retinal diseases using the ResNet and U-Net models has various applications in ophthalmology and healthcare:

Early Disease Detection: Crucial for timely intervention and treatment of retinal diseases like diabetic retinopathy. Screening Programs: Automating classification can facilitate large-scale screening for at-risk populations. Patient Triage: Automated systems can prioritize patients based on disease severity, ensuring critical cases are seen promptly. Research and Clinical Trials: Analyzing large datasets of retinal images can aid in identifying patterns and trends in disease progression. Clinical Decision Support: AI-based systems can provide ophthalmologists with additional insights for diagnosis and treatment decisions.

📌 Conclusion The integration of Quantum Transfer Learning with classical machine learning models marks a significant advancement in the detection and classification of Diabetic Retinopathy. By leveraging the strengths of models like ResNet and U-Net, this project demonstrates enhanced accuracy and efficiency in diagnosing DR from retinal fundus images.

The results indicate that our proposed methodology not only improves classification performance—achieving up to 97% accuracy—but also streamlines the process, making it more accessible for healthcare providers. This dual approach of employing Quantum Transfer Learning alongside traditional techniques promises a future where early detection and intervention for diabetic retinopathy can be achieved at a larger scale, ultimately aiming to reduce the burden of vision loss among diabetic patients.

Future work will focus on refining these models further, expanding the dataset for training, and exploring additional applications of Quantum Transfer Learning in other medical imaging fields.
