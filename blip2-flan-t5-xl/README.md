# Image Captioning: BLIP2 Flan-T5-XL Model
Contributor: Vagdevi Sahasra Bandaru

## Data
### Data for pre trained model testing:
* Reference Folder: img-test
* Reference Folder: images

## Model
Hugging Face: Salesforce/blip2-flan-t5-xl

## Files
### README
This readme file has the explanations to all the files in the folder along with steps for code execution.

### blip2_flan_t5_xl_model_test.ipynb
This is IPython Note Book file for testing pre trained blip2-flan-t5-xl model by Salesforce on images from 'images' and 'img-test' folders.

# Steps for Executing the files
### Testing Pre Trained Model from Salesforce
1. Upload the 'blip2_flan_t5_xl_model_test.ipynb' file to colab and make sure it is running on L4 GPU.
2. Upload the images from the 'img-test' and 'images' folder to colab for testing the model on unseen data.
3. Connect to runtime and run all cells.
4. The captions for the uploaded images are generated and printed for reference.

# Github Repositiories of BLIP models by Salesforce
* [BLIP](https://github.com/salesforce/BLIP)
* [BLIP2](https://github.com/salesforce/LAVIS)

# Citations
[1] Li, Junnan, et al. "Blip: Bootstrapping language-image pre-training for unified vision-language understanding and generation." International conference on machine learning. PMLR, 2022.

[2] Li, Junnan, et al. "Blip-2: Bootstrapping language-image pre-training with frozen image encoders and large language models." International conference on machine learning. PMLR, 2023.
