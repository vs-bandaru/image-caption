# Image Captioning: BLIP Image Captioning Large Model
Contributor: Vagdevi Sahasra Bandaru

## Data
### Data for pre trained model testing:
* Reference Folder: img-test

### Data for fine tuning:
* Testing Data: 
  - Hugging Face: irodkin/celeba_with_llava_captions
* Testing Data: 
  - Reference Folder: celebA_data

### Data for fine tuned model testing:
* Reference Folder: images

## Model
Hugging Face: Salesforce/blip-image-captioning-large

## Files
### README
This readme file has the explanations to all the files in the folder along with steps for code execution.

### blip_large_model_test.ipynb
This is IPython Note Book file for testing pre trained blip-image-captioning-large model by Salesforce on images from 'img-test' folder.

### BLIP_Image_Caption_Large_CelebA.ipynb
This is IPython Note Book file for fine tuning the blip-image-captioning-large model by Salesforce on the Hugging Face celeba_with_llava_captions dataset.

### fine_tuned_blip_large_celeba.zip
This is the blip-image-captioning-large model fine tuned on the celeba_with_llava_captions dataset saved a zip for testing.

### BLIP_Large_CelebA_Test.ipynb
This is IPython Note Book file for testing the fine tuned blip-image-captioning-large model different example input images.

# Explanation
The code files in this folder implement the process of fine tuning BLIP's image captioning model on CelebA dataset.
The following are the specifics of the implementation:
1. Model: blip-image-captioning-large
2. GPU: L4 GPU
3. Data Size: 4000
4. Batch Size: 8
5. Train Split: 70%
6. Val Split: 15%
7. Test Split: 15%
8. Epochs: 4
9. Optimiser: AdamW 
10. Learning Rate: 1e-5

# Steps for Executing the files
## Testing Pre Trained Model from Salesforce
1. Upload the 'blip_large_model_test.ipynb' file to colab and make sure it is running on L4 GPU.
2. Upload the images from the 'img-test' folder to colab for testing the model on unseen data.
3. Additionally, if you want to upload an image of your own choice, upload it too.
4. Connect to runtime and run all cells.
5. The captions for the 3 images from 'img-test' folder are generated and printed for reference.
6. Additionally, based on the captions predicted by the model, I have generated images by using the captions as prompts to ChatGPT for comparison.
7. If you have an input image of your choice then you need to uncomment the last line at the end of examples section and run the last cell to generate caption for your choice of input image.

## Fine Tuning
1. Upload the 'BLIP_Image_Caption_Large_CelebA.ipynb' file to colab and make sure it is running on L4 GPU.
2. Upload the 4 images from the 'celebA_data' folder to colab.
3. Connect to runtime and run all cells.
4. The model takes time to process the epochs.
5. After completion of processing, the model is saved in a 'fine_tuned_blip_large_celeba.zip' format which is downloadable.
6. The captions for the 4 images from celebA_data' folder are generated and printed along with ground truth captions for reference.

## Testing Fine Tuned Model
1. Upload the 'BLIP_Large_CelebA_Test.ipynb' file to colab and make sure it is running on L4 GPU.
2. Upload the saved model 'fine_tuned_blip_large_celeba.zip' to the colab.
3. Upload the 8 images from the 'images' folder to colab for testing the model on unseen data.
4. Additionally, if you want to upload an image of your own choice, upload it too.
5. Connect to runtime and run all cells.
6. The '.zip' folder is unzipped and the fine tuned model and process are loaded.
7. The captions for the 8 images from 'images' folder are generated and printed for reference.
8. Additionally, based on the captions predicted by the model, I have generated images by using the captions as prompts to ChatGPT for comparison.
9. If you have an input image of your choice then you need to uncomment the last line at the end of examples section and run the last cell to generate caption for your choice of input image.

# Github Repositiories of BLIP models by Salesforce
* [BLIP](https://github.com/salesforce/BLIP)
* [BLIP2](https://github.com/salesforce/LAVIS)

# Citations
[1] Li, Junnan, et al. "Blip: Bootstrapping language-image pre-training for unified vision-language understanding and generation." International conference on machine learning. PMLR, 2022.

[2] Li, Junnan, et al. "Blip-2: Bootstrapping language-image pre-training with frozen image encoders and large language models." International conference on machine learning. PMLR, 2023.
