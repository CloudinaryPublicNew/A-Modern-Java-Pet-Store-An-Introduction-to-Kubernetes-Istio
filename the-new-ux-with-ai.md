# The new UX with AI — the Android app with IBM Watson

I was inspired by Shazam application for music. Alike with Shazam for music one could point a smart phone on a pet, take a picture and get the name / breed of an animal, with the price quote from our pet store.

How to do it? First I need to classify what is on the picture. The IBM Watson Visual Recognition service is pretty awesome in classification of the animals. There is a quite robust classification of dogs, with their breeds. There are other animals classifiers as well. I need an[http://bluemix.net](http://bluemix.net/) IBM Cloud account, and I need to provision the Watson Visual Recognition service for that. That is easy.

Some time ago I have created a selfie app for Android \(you can get the [https://github.com/blumareks/cloudinary-watson/tree/master/lab2](https://github.com/blumareks/cloudinary-watson/tree/master/lab2)← Smart Selfie app here\), so I reused the same code tailoring it for the purpose of our Shazam for pets AI powered app. The Android app GitHub is here: [https://github.com/blumareks/2018-petstore-android](https://github.com/blumareks/2018-petstore-android)

In addition to the IBM Watson Visual Recognition, I added [https://console.bluemix.net/catalog/services/text-to-speech](https://console.bluemix.net/catalog/services/text-to-speech)→IBM Watson Text to Speech service — so kids could get the information faster without reading it \(they love Voice UI I noticed\).

Finally you need to copy the above mentioned credentials from those Watson services, and paste them in the credentials.xml file of this Android app.

Please visit my GitHub repo to learn more and see the videos on how to do it:[https://github.com/blumareks/2018-petstore](https://github.com/blumareks/2018-petstore)

Please follow me on the twitter:[https://twitter.com/blumareks](https://twitter.com/blumareks)



