# Convert a picture into a drawing/painting with Gimp

### Introduction
This tutorial describes how to use some aspects of Gimp to convert a picture into a drawing. Useful to insert the drawing in a comic or to avoid problems of copyright ;)
In this example, we start with the following picture of a temple in Seoul, Korea. Then, I will guide you step by step to turn this picture into a drawing. 

![alt text](https://github.com/martraire/PhotoToSketch/blob/master/images/Seoul.jpg)

Basically, it is a two-steps process:
  * First, we extract the outlines of the drawing (black lines),
  * Then, we focus in filling it with colors. 
  
Concretly, we use a layer for each element: one that contains the lines of the drawing and another one containing the colors. Let's start !


### 1. Drawing the outlines of the drawing
#### Extracting the outlines of the drawing
Once your photo is opened with Gimp, Duplicate the layer that contains the photo using the menu: **layer > duplicate layer** or the icon in the menu dedicated to the layers. When duplicated, you should have 2 layers in your menu (cf. the following picture, i renamed my 2 layers: Outlines & Colors).

![alt text](https://github.com/martraire/PhotoToSketch/blob/master/images/Step1.jpg)

Now, we are going to extract the outlines of the image. Activate the layer above and then select **Filters > Border Detection > Outline**.
For this example, the *"Sobel" algorithm with a quantity of 1.0* works well. Of course, it is up to you to see which setting is the most appropriate to your image. 

![alt text](https://github.com/martraire/PhotoToSketch/blob/master/images/Step2.png)


#### Cleaning and improving contrasts

After confirmation, you get a predominantly black image with white plots. There are still traces of colors: you get rid of it by passing the image in black and white: menu **Colors > Desaturation**. In the black-and-white option window, choose "brightness" and confirm.

Now, it is time to clean the layer that contains the lines to remove all unnecessary traces. For this, we increase the contrasts considerably by using the curves: menu **Colors > Curves**. In the window, distort the curve in this way:

![alt text](https://github.com/martraire/PhotoToSketch/blob/master/images/Step3.png)

N.B: I strongly advise you to spend some time learning and understanding the curved tool. It is truly an indispensable tool for photo editing. Once you know how to use it, you will not be able to do without it !

At this point you should get this:

![alt text](https://github.com/martraire/PhotoToSketch/blob/master/images/Step4.png)


#### Inverting color and making the background transparent

Then, we invert the colors to have black lines on white background: menu **Colors> reverse**.

We must change the white background as transparent. To do this, we add a layer mask: right click on the layer then choose *"add a layer mask"*. In the window, select *"Copy the layer in grayscale"* and check *"invert the mask"*.

![alt text](https://github.com/martraire/PhotoToSketch/blob/master/images/step5.png)

At the end of the first part, we have finished with the drawing. Now, let's work on the background colors.


### 2. Color processing
#### Adding a filter

We select the second layer, renamed "colors", and apply a paint effect: menu **Filters> Artistic> Oil Painting**. The size of the mask corresponds to the grain size of the paint, so choose a size large enough for the colors to give the impression of drooling. I invite you to test a combination of parameters according to what you want to get. Here are the settings for the photo of the example:

![alt text](https://github.com/martraire/PhotoToSketch/blob/master/images/Step6.jpg)

#### Saturation and brightness 
To finish, we give an artificial appearance to the colors to get closer to a watercolor effect. We will increase the brightness (to give the impression of dilution of the color) and increase the saturation (to make the colors more artificial).

From the **Colors> Hue-Saturation** menu, set the *brightness to 40* and *increase the saturation to 100*.

![alt text](https://github.com/martraire/PhotoToSketch/blob/master/images/Step7.jpg)

Finally, here is the result :

![alt text](https://github.com/martraire/PhotoToSketch/blob/master/images/Step8.jpg)

And a last one comparing our drawing with the original picture:

![alt text](https://github.com/martraire/PhotoToSketch/blob/master/images/FinalComparison.jpg)
