# The name is Rein.

A Documentation / Research For LLms and Transformers.


## Content
- [Stable Diffusion](#stable-diffusion)
- Transformers
- LLm
- LangChain
  
# Stable Diffusion
The primary function of Stable Diffusion is to generate detailed images based on text descriptions, but it can also be used for other tasks like inpainting, outpainting, and creating image-to-image translations guided by text prompts. Its weights, model card, and code are available publicly.

## Working
- Starts with noise then start reducing the noice on each iteration.
- Text-to-Image Process in 4 parts
    1. Image Encoder converts training images into vectors in a mathematical space known as the latent space, where image information can be represented as arrays of numbers.
    2. A Text Encoder translates text into high-dimensional vectors that machine learning models can comprehend.
    3. Diffusion Model then utilizes the text guidance to create new images in the latent space.
    4. Finally, an Image Decoder transforms the image data from the latent space into an actual image constructed with pixels.
   
## Terms and Params 
- CFG scale : The CFG scale essentially governs how closely the generated image adheres to the user's prompt or input image.
- Denoising : how much image should change.
- Textual Inversion : min 12 gb vram, Fine tuning the model
- Sampling methods : 
- Latent nothing : part of mask gets blend with background.
  
## Prompt Engineering
- **More Detailed Image** :  Wallpaper, hyperrealism, poster, sharpfocus, insanely detailed, filigree, intricate,perfectionism, max details, 4k, HQ angelic, decorations, masterpiece, hard edge, breathtaking, embroidery.
- **Lighting** : Studio lighting, diffused lightening, cinematic.

## Fine Tunning Training
Textual inversion to be used for fine-tuning the model on custom dataset. ( min. GPU 12 GB vram )
## For Online training 
- [Dream booth Colab](https://colab.research.google.com/github/ShivamShrirao/diffusers/blob/main/examples/dreambooth/DreamBooth_Stable_Diffusion.ipynb)