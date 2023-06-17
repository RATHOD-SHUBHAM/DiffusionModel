# DiffusionModel

Diffusion models are deep generative models that work by adding noise (Gaussian noise) to the available training data (also known as the forward diffusion process) and then reversing the process (known as denoising or the reverse diffusion process) to recover the data.

## 1] SAM_SD

``` Segment Anything Model + Stable Diffusion ```

I used the Segment Anything model, to create a mask for an image, and then I used stable diffusion to change the background based on the mask.

#### Steps:

1. Set up the environment:
   - Make sure you have Python installed on your system.
   - Install the necessary libraries, including PyTorch, NumPy, and torchvision.

2. Mask Generation with SAM:
   - Download and set up the SAM implementation library.
   - Import the required modules and functions from the SAM library.
   - Load the pretrained SAM model or train it on your dataset if needed.
   - Prepare the input image for mask generation.
   - Feed the image into the SAM model to obtain the generated masks.
   - Process the generated masks as desired.

3. Preprocess the Image and Masks:
   - If the input image is not in the required format for stable diffusion, preprocess it accordingly.
   - If necessary, resize the generated masks to match the dimensions of the image.

4. Background Replacement with Stable Diffusion:
   - Download and set up a stable diffusion implementation library.
   - Import the necessary modules and functions from the diffusion library.
   - Prepare the preprocessed image and masks as input for stable diffusion.
   - Define the diffusion parameters, such as diffusion steps, time steps, and noise schedule.
   - Use the diffusion model to iteratively modify the image based on the masks.
   - Update the image's background according to the mask values during each diffusion step.

<img width="1546" alt="Screenshot 2023-06-17 at 1 51 11 AM" src="https://github.com/RATHOD-SHUBHAM/DiffusionModel/assets/58945964/9dd654d4-cb37-44e8-8f45-40b91405e90e">

---
  
## 2] Stable diffusion to generate images:

1. Set up the environment:
   - Install the necessary libraries, including PyTorch, NumPy, and torchvision.
   - Download and set up a stable diffusion implementation library.

2. Define Diffusion Parameters:
   - Set the diffusion parameters.
   - The number of diffusion steps determines the level of image generation. More steps lead to finer details but take longer to compute.
  
3. Generate Images:
   - Import the necessary modules and functions from the diffusion library.
   - Create an instance of the diffusion model with the desired parameters.
   - Prompt to images.
   - Generate images by iteratively applying the diffusion steps.
   - Save the generated images to disk or store them in memory for further analysis or applications.


<img width="1097" alt="Screenshot 2023-06-17 at 3 11 02 AM" src="https://github.com/RATHOD-SHUBHAM/DiffusionModel/assets/58945964/e231f013-93ab-49a8-b29a-d1213425d0b0">

---
