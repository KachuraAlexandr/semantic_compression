# semantic_compression
The implementation of the algorithm for semantic compression of an image with DALL·E 2.

To perform semantic compression:
1. Download the weights for the [prior](https://huggingface.co/laion/DALLE2-PyTorch/blob/main/prior/best.pth), the [decoder 1](https://huggingface.co/laion/DALLE2-PyTorch/blob/main/decoder/v1.0.2/latest.pth) and the [decoder 2](https://huggingface.co/Veldrovive/upsamplers/resolve/main/working/latest.pth) and place them in the directory `./weights`.
   Rename the weights for the prior to `prior_best.pth`, the decoder 1 - to `decoder_latest.pth`, the decoder 2 - to `decoder_2_latest.pth`. 
2. Place the images in the directory `./data/images` and the captions in the directory `./data/captions`.
3. Install the suggested versions of python modules with the command `pip install -r requirements.txt`.
4. Run all the cells of the notebook `semantic_compression.ipynb`.
5. The mean value of RGB-PSNR of the maximum values of RGB-PSNR among all the captions of each image will be output in the final cell. 
