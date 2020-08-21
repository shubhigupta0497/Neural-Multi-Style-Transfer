# Neural-Multi-Style-Transfer

Nueral Style transfer is an optimazartion technique used to take two image - content image(subject) and style reference. We blend them together so o/p looks like the content image but has the style of the reference image. Tensorflow is used to implement this in python. The algorithm works on the principle that distance original and final output is the loss and our aim is to minimise the loss to match the iput as much as possible. 

Losses considered can be categorised into two - 
1. Content Loss - how different is the content of the two images
2. Style Loss - difference between the two images in terms of their style.

We try to transform the input image to minimize the content distance with its content image and style distance with its style image using loss functions as - 
We use the vgg19 image classification technique to generate feature vector of all the images and reduce style and content loss to generate output image. We extended are project for multiple styles so the outtput image not only rendered one style but a combination of styles. For this we calculated to losses from each individual styles and used it match the output image.
