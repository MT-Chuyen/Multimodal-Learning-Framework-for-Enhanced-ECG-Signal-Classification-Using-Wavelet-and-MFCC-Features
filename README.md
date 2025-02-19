# Multimodal-Learning-Framework-for-Enhanced-ECG-Signal-Classification-Using-Wavelet-and-MFCC-Features

Authors: Assoc. Prof. Vu-Anh Tran, Chuyen-Tat Mai, Anh-Thi Diem Nguyen

## Project Goals:

**Problem Statement:** Accurate classification of cardiac arrhythmias is crucial for managing cardiac disorders, but manual analysis of ECG data is challenging due to limited expertise and the volume of data.

**Importance:** Leveraging machine learning to automate ECG analysis is a promising solution to improve diagnostic efficiency and reduce resource burden.

**Specific Objectives:**

*   Develop a novel multimodal learning framework for ECG signal classification.

*   Integrate wavelet-transformed features and MFCC features to capture complementary information.

*   Improve classification accuracy and robustness compared to existing methods.

*   Demonstrate generalizability across different ECG datasets (MIT-BIH Arrhythmia Database (MITDB) and MIT-BIH Atrial Fibrillation Database (AFDB)).

**Target Audience:** Cardiologists, healthcare professionals, and researchers in cardiac arrhythmia detection.

## Methodology:

**Core Components:**

*   Multimodal Approach: Combining both wavelet-transformed features (time-frequency) and MFCC features (spectral).

*   Wavelet Branch: Wavelet extraction to capture time-frequency information, followed by a 1D DCNN and BiLSTM for temporal dependencies.

*   MFCC Branch: MFCC features processed by a 2D CNN to capture spectral characteristics.

**Technical details:**

*   ECG signals undergo pre-processing for noise reduction and baseline correction, ensuring data quality.

*   Both Feature branches (MFCCs and Wavelets) are extracted from ECG signals, optimizing the models' ability to capture intricate patterns

**Datasets:**

*   MIT-BIH Arrhythmia Database (MITDB) : Used five classes for heart beats: normal (NOR), left bundle branch block (LBBB), right bundle branch block (RBBB), atrial premature beats (AP), and premature ventricular beats (PVC).

*   MIT-BIH Atrial Fibrillation Database (AFDB) : Used four heartbeat classes: atrial fibrillation (AFIB), atrial flutter (AFL), atrioventricular rhythm (AVR), and normal sinus rhythm (NSR)

**Training and settings:**

*   Model trained using Adam optimizer with an learning rate of 0.001

*   Implemented a learning rate decay (reduce learning rate by 10 every 16 epochs)

*   Framework is built using TensorFlow and Keras framework

**Model evaluation:**

*   Testing on both dataset to ensure framework robustness

## Results:

**Key Metrics:** Classification accuracy.

**Core performance:**

*   MITDB: Achieved a classification accuracy of 99.70%.

*   AFDB: Achieved a classification accuracy of 99.44%.

**Core finding:** Results show that the proposed learning framework provides significant accuracy and robustness to address the challenges of noise inference.

**Wavelet selection analysis:** Experiment showed the importance to choose and hyper-tune parameters for different wavelet to synergy and enhance performance

**Comparison to strategy:** The model were trained in several strategies, then the accuracy of different model strategies were compared, and the best model was chose

## Individual role
_I significantly contributed to the success of this study. The development and testing of the multimodal framework were guided by my key ideas, such as proposing improvements to the original BiLSTM network, integrating MFCC features to improve accuracy and robustness, and incorporating multimodal learning framework by incorporating wavelet processing in parallel. I was instrumental in the coding and implementation, I undertook responsibilities in dataset preprocessing, MFCC and Wavelet feature engineering, model construction to implement parallel streaming of data, model choice, training and evaluation in various scenarios including "BiLSTM only," "BiLSTM + Wavelet," "BiLSTM + MFCCs," and "BiLSTM + Wavelet and MFCCs in parallel." I also led the integration of various CNN and BiLSTM backbone models. I participated actively in writing the research manuscript._
