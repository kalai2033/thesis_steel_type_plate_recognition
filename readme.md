This repository consists of the codes used for the completion of master thesis 'Improving character recognition of engraved/embossed steel type plate using GAN generated image'. 

The description of each folder and its subfolder is given below :

1) ConsolidatedResultsofOCRandGAN

	It consists of qualitative evaluation of GAN. The subfolders contains the corresponding GAN translated images.

a) ann - annotated
b) cyc - CycleGAN
c) fac - FactorGAN
d) ori - Original
e) pix - Pix2pix
f) synth - Pix2pix + synthetic data

The complete results can be accessed using the Results.html file.

Also the evaluation of OCR is provided in this folder.

a) ocr.xlsx consists of bar graphs and tables obtained from the output of OCR
b) OCReval.docx contains the output of both the google vision OCR and the proposed OCR with these test images.


2) CycleGAN-and-pix2pix

This folder contains the training codes for both the pix2pix and the cycleGAN. It is cloned from https://github.com/junyanz/pytorch-CycleGAN-and-pix2pix. The
license file is also provided. 

The xxx.pth files are the best generator files obtained for corresponding GAN.
The training graphs, logs, some trained models and its results for both the pix2pix and cycleGAN are also available in the folder.

3) FactorGAN

This folder contains the training codes for FactorGAN. It is cloned from https://github.com/f90/FactorGAN. The
license file is also provided. 

The FactorGAN_generator.pth is the best generator files obtained for FactorGAN.
The training graphs, logs, some trained models and its results for FactorGAN are available in the results folder.

4) Latex_codes
It consist of the code used for writing the thesis report. The final report is provided as pdf.

5) ProposedOCRengine

This folder contains the codes for the proposed OCR engine. It integrates the model for text detection and text recognition.
This is modified from the two repositories : i) text detection https://github.com/clovaai/CRAFT-pytorch and 
ii) text recognition https://github.com/clovaai/deep-text-recognition-benchmark. Their license files are also provided.

The evaluation of extraction of text is shown in MyOCR.ipynb file. To extract text from a image, use the extracttext.py with the path of the image as a argument.


6) Pytorch-fid

This folder contains the code for FID evaluation. It is cloned from https://github.com/mseitzer/pytorch-fid and is provided with its license.

7) Jupyter notebook files

a) Creation_of_dataset_pairs.ipynb - Code for generation of image pairs. Finding duplicates, resizing, RGB to grayscale, difference and thresholding

 
b) Extraction_of_texts_using_google_vision_api.ipynb - code for integrating google vision api for extracting texts


c) GAN_Synthetic_Images_creation - Code for generation of synthetic dataset


d) Quantitative_Evaluation.ipynb - code for quantitative evaluation metrics such as MSE and SSIM measures


e) Scraping_From_google_Images.ipynb - code for web scraping of steel type plate images
