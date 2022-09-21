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

### My inputs
![cat](https://user-images.githubusercontent.com/50231750/191466407-6fbb8a4c-a3f1-4626-a5f1-5764b656fafc.jpg)
![drop-of-water](https://user-images.githubusercontent.com/50231750/191466446-2aa88a41-77a7-4e6d-b8e2-e6642f09580b.jpg)


## Output
The output would be a sequence of images taken at different iterations and would be stored in the `output/` directory, you can change the number of iterations and images to play around

### My output
![generated_image](https://user-images.githubusercontent.com/50231750/191466533-724e6932-e095-4291-8b1f-d534c9a31854.jpg)

## Generated Video

https://user-images.githubusercontent.com/50231750/191467062-9650b9d3-9696-469a-970d-5d0a9cd59be6.mp4

