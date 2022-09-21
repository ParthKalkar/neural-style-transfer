# neural-style-transfer
This repository contains the code for implementation of the Neural Style Transfer Algorithm. 

## Art in Deep Learning: Neural Style Transfer

In this notebook, we will learn about Neural Style Transfer. This algorithm was created by Gatys et al. (2015) (https://arxiv.org/abs/1508.06576). 

**In this notebook, we will:**
- Implement the neural style transfer algorithm 
- Generate novel artistic images using our algorithm 

Most of the algorithms you've studied optimize a cost function to get a set of parameter values. In Neural Style Transfer, you'll optimize a cost function to get pixel values!

## Code
The code follows a step-step implementation and all the details are mentioned in the jupyter code file. The notebook is performed as an assignment therefore has some tasks in the end for someone to try

## Model
We use the pretrained model - 'imagenet-vgg-verydeep-19', the model can be downloaded using the following command: 

`!wget --output-document=imagenet-vgg-verydeep-19.mat 'https://storage.googleapis.com/marketing-files/colab-notebooks/style-transfer/imagenet-vgg-verydeep-19.mat'`

## Run
There are two ways to run the code: 

**Run using Colab**: 
  1. Download the jupyter notebook, images folder and create a output folder 
  2. Load in Google colab 
  3. connect to GPU runtime 
  4. Run all cells.
**Note:** The code is suitable for tensorflow version 1.15 therefore the previous version should be uninstalled and the new version should be installed.
To do that, use the following command: 

`!pip uninstall tensorflow==2.8.2`

`!pip install tensorflow==1.15`

**Run using python script**: 
  1. Create a project folder 
  2. Download the nst_generate.py file on your laptop in the same folder 
  3. Download the images folder and create an output folder 
  4. Open the terminal and run the following command : `python3 nst_generate.py my_content.jpg my_style.jpg gen.jpg`
**Note:** You should have the following libraries installed: NumPy, Pandas, Imageio, Tensorflow, Sklearn, CV2

To do that, just run the following command: 

`pip install name_of_the_library`

## Inputs
The program expects a `content_image` and `style_image`, the size of the images should be same either `300*225` or `400*300`. You can resize the images or find them online

## Output
The output would be a sequence of images taken at different iterations and would be stored in the `output/` directory, you can change the number of iterations and images to play around


