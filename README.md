# Road-Network-Extraction-from-Satellite-Imagery
# Some of the prediction results from test folder images.
![image](https://github.com/user-attachments/assets/0728f535-dc94-4adc-814b-f00efc8ffb72)
![image](https://github.com/user-attachments/assets/66e3dbeb-3f63-450c-b10b-40a211803881)
![image](https://github.com/user-attachments/assets/2dd316d9-6258-4d09-b752-f8d706e7235f)
![image](https://github.com/user-attachments/assets/f8a329fb-1139-4790-99ff-05d44f470068)

# 1. Approach
The approach for the road network extraction from satellite imagery involves the following steps:

  # 1. Data Loading and Preprocessing:
  - Used randomly selected 512 images from train folder for training as I don't have high computational powered system 
  - The images and corresponding mask files are loaded from the specified directory.
  - Images are resized to a fixed size (512x512) and normalized to a range of [0, 1].
  - Masks are also resized and binarized (converted to binary values).
  
  # 2. Data Splitting:
   - The dataset is split into training and validation sets using an 80-20 split.

# 2. Model Architecture
- The model used is a U-Net, which is a common architecture for image segmentation tasks. The U-Net consists of an encoder-decoder structure with skip connections.
- Use a custom combined loss function (Binary Crossentropy + Dice Loss).
