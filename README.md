# Converting Image to pencil sketch with python cv2 library

I have made this project as a a part of my data science internship at @LetsGrowMore (LGM).

The steps followed are :
- Loading the Image.
- Converting to grayscale.

Gray scale conversion is important for multiple reasons like;
Dimension reduction, Reduced model complexity & for some algorithms to even work (as many algorithms are customized to work only on grayscale images)

- Inverting the image.
  
Images are represented using RGB or Red Green Blue values. Each can take up an integer value between 0 and/or 255. For example, a red color is represent using (255, 0, 0), white with (255, 255, 255), black with (0, 0, 0), etc.
Inverting an image means reversing the colors on the image. For example, the inverted color for red color will be (0, 255, 255). Note that 0 became 255 and 255 became 0. This means that inverting an image is essentially subtracting the old RGB values from 255.

- Gaussian Blur.

Gaussian blurring is highly effective in removing Gaussian noise from an image.
We should specify the width and height of the kernel which should be positive and odd. We also should specify the standard deviation in the X and Y directions, sigmaX and sigmaY respectively.

- Dodging and Burning
  
It is used to get the final output. These refer to techniques employed during the printing process in traditional photography. We can refer Dodging lightens an image, whereas burning darkens it.
