# augment-training-photo
## A Notebook to augment your own image files to increase your training data for a neural network

This code will help you to create .jpg photos which all have the same size to use them to train a neural network. Therefore you can use your own photos and converte them in the size you need for your network. Additionally we create more photos from every class to augment the training data available.

1. you need a special folder structure to process the images the same way as myself (of course you can change my code to use a your own folder structure). My folder structure is the following.
 * _Projectfolder_ (in the code you will see that this is the root folder for my operations)
   * _training_ (folder which contains the training classes)
     * _class1_ (store here the photos which you want to use for training the network. Every photo will get a size which you define and if there are not enough photos for training from a class we will augment the photos available)
     * _class2_
     * _classXX_
2. The code will ask which size your training photos for the network should have
3. The Code will find the biggest width/ height of all photos in every training class
4. Every photo will be squared in every training class (e.g. 500x500 pixel if the biggest width/ height was 500 pixel of your training photos in a certain class)
5. Every photo which is smaller than the biggest width/ height will keep the old size but gets a black border to reach consistent size for every photo
6. Every photo will get the size which you want to train your network
7. Flip every image left-right in every class to double the training pictures in every class
8. Rotate the trainings pictures one (to five) degree clock wise and counter clock wise to create new photos for training
