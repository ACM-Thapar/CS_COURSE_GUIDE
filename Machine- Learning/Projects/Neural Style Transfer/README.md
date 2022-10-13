
# Neural Style Transfer & Neural Doodles
This tutorial uses deep learning to compose one image in the style of another image (ever wish you could paint like Picasso or Van Gogh?). This is known as _neural style transfer_ and the technique is outlined in [A Neural Algorithm of Artistic Style](https://arxiv.org/abs/1508.06576) 
## Setup
- Download the [imagenetvggverydeep19mat](https://www.kaggle.com/datasets/teksab/imagenetvggverydeep19mat) to perform the transfer learning task and place it in the ``pretrained-model/imagenet-vgg-verydeep-19.mat``
- Add desired content and  style images into the ``images `` 

## Guide

This is implemented by optimizing the output image to match the content statistics of the content image and the style statistics of the style reference image. These statistics are extracted from the images using a convolutional network.
# Examples

What if Monalisa was printed by Van Gough 

<img src="https://upload.wikimedia.org/wikipedia/commons/thumb/e/ec/Mona_Lisa%2C_by_Leonardo_da_Vinci%2C_from_C2RMF_retouched.jpg/405px-Mona_Lisa%2C_by_Leonardo_da_Vinci%2C_from_C2RMF_retouched.jpg" alt="Monalisa" width="200"/>
<a href="https://www.freepnglogos.com/pics/plus-icon" title="Image from freepnglogos.com"><img src="https://www.freepnglogos.com/uploads/plus-icon/plus-icon-plus-math-icon-download-icons-9.png" width="250" alt="plus icon, plus math icon download icons" />
<img src="https://upload.wikimedia.org/wikipedia/commons/thumb/4/4c/Vincent_van_Gogh_-_Self-Portrait_-_Google_Art_Project_%28454045%29.jpg/330px-Vincent_van_Gogh_-_Self-Portrait_-_Google_Art_Project_%28454045%29.jpg" alt="Van Gough" width="200"/>

<hr>

 - First of all the we need to make it so that the image will fit into our CNN which can handle 400x300 image size.
 - This resizing is done with the help of opencv as it will not lessen the quality of the image too much while also producing good results.
 - Next we will add some noise to the image to actually make it transform into another style 
 - Running it for the number of iterations you want until one gets the desired results
 <hr>
 
 ### Output
 ![enter image description here](https://cdn.discordapp.com/attachments/991747075404472344/1030047399906902036/thumbnail.png)
