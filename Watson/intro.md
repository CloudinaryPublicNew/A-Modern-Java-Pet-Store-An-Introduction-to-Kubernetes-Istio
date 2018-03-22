# Getting Started with IBM Watson Visual Recognition & Cloudinary

####Creating Visual Recognition custom models

You can create IBM Watson Visual Recognition custom models, trained with your own images, to suit your specific visual recognition needs. This topic describes how to use the Visual Recognition model builder in IBM Watson Studio to create a custom model.



#### Before you begin {#before-you-begin}

[Set up your project](https://dataplatform.ibm.com/docs/content/analyze-data/visual-recognition-setting-up.html)to use the Visual Recognition model builder.



#### Procedure {#procedure}

1. [Prepare your images](https://dataplatform.ibm.com/docs/content/analyze-data/visual-recognition-prepare.html)
 
   Collect a minimum of 10 images for each class in ZIP \(.zip\) files, and then upload them to your project.
   
We'll use Cloudinary to source and organize our training images.

![](/assets/media-library.png)
   
   
To simplify your efforts you can use Cloudinary's media library upload tool to source images from the internet.  For example you can restrict your search to image that are tagged as free to use, even commercial.

![](/assets/rights.png)

In addition, you can also set the public id of the images, folder location and set tags:

![](/assets/media-search.png)

Simply select similar images and click the upload button:
![](/assets/select.png)

Finally, to build a zip file of images for each class, search by tag and select the images you want to include in your zip file. Click the download and a zip file of those selected images will be downloaded.

![](/assets/download-zip.png)


2. [Train your custom model](https://dataplatform.ibm.com/docs/content/analyze-data/visual-recognition-train.html)
 
   In the Visual Recognition model builder, define your classes and add images.
 
3. [Test your trained model](https://dataplatform.ibm.com/docs/content/analyze-data/visual-recognition-test.html)
 
   After your model is trained, you can use the
   **Test**
   area of the model builder to classify test images using your custom model.
 
4. [\(Optional\) Retrain your model](https://dataplatform.ibm.com/docs/content/analyze-data/visual-recognition-retrain.html)
 
You can improve the performance of your model by adding or removing training images and then retraining the model.
 



  




