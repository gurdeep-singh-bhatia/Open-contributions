# Hello forks, i am Gurdeep Singh and today we will learn about image blending :smile:

## First of all we would like to cover the add() function of open cv. Now we know that images are saved in matrix form of pixels and when we add two images then it means that we are adding matrices 

So like wise add() function add two matrices ie two images. Now in order to get some transparency and some different importance/weightage to diff images then concept of blending comes which is special form of adding two images which has the following formula :

***g(x) = (1 - a)f(x) + af1(x)*** 

Also blending is very important when we want to extract some important features out of an image 

**We can also blend an image ie add an image with its blur version too to get some important features extracted**

![img](https://i.stack.imgur.com/kl3Md.jpg)

**The above image is an original image**

![img](https://i.stack.imgur.com/xf84j.jpg)

**The above is the blended version of the previous image**

And the code of above image is simple:

processed_image=cv2.addWeighted ( 1stimage,4, cv2.GaussianBlur( 1stimage , (0,0) , 250/10) ,-4 ,128) # blending technique 


Thanks 

For further query connect me on linkedin: [linkedin](https://www.linkedin.com/in/gurdeep-singh-bhatia-319441171/)
