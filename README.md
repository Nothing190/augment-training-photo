# augment-training-photo
## A Notebook to augment your own image files to increase your training data for a neural network

This code will help you to create .jpg photos which all have the same size to use them to train a neural network. Therefore you can use your own photos and converte them in the size you need for your network. Additionally we create more photos from every class to augment the training data available.

1. you need a special folder structure to process the images the same way as myself (of course you can change my code to use a your own folder structure). My folder structure is the following.
 * _Projectfolder_ (in the code you will see that this is the root folder for my operations)
   * _training_ (here you can save your original .jpg photos)
    * * _class1_ (here the code will save the .jpg photos with the new size for the neural network)
    * * _class2_
