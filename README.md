# Project Title
Monthly Image base Question and Answering AI Competition

# Project Overview
Multimodal AI is a technology that combines different types of data, such as text and images, to comprehensively handle a wide range of applications. It can convert images into text and generate images based on text, among other uses. It offers high value in terms of service and challenges the development and advancement of multimodal AI models.

# Competition Participation
- Rank
  - public : 12/536
  - private : 11/536

## Data Sources
The project uses the following data sources:
- 'image/train' : Training data
- 'image/test' : Test data 
- `train.csv`: Training data
- `test.csv`: Test data
- if you want to get datas, please visit (https://dacon.io/competitions/official/236118/data)

## Data Preprocessing
- The model utilizes the VQADataset class to process data. This class loads and preprocesses images and questions from a DataFrame. Additionally, it applies data augmentation to image data using RandAugment.

## Model
- Our multimodal AI model, based on the VILT architecture, excels at processing both text and image data. This model leverages the power of vision and language understanding to perform tasks such as image captioning, visual question answering, and more.
- Kim, W., Son, B., & Kim, I. (2021). ViLT: Vision-and-Language Transformer Without Convolution or Region Supervision. In ICML 2021 Long Presentation. Retrieved from https://arxiv.org/abs/2102.03334

## Model Training
The training and evaluation processes are as follows:

Model Training: The train function is used to train the model. It processes mini-batch data and updates the model using an optimizer and scheduler.

Inference: The inference function is used to perform inference with the trained model. This function generates predictions for input data.

## ViLT-base-VQA.ipynb
If you want to run the code, please see the 'ViLT-base-VQA.ipynb'



