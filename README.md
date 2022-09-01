# Create images that contain other images(mosaic effect)

I tried to learn it and use it as my profile photo
<br>
This script is based on the [artcle](https://towardsdatascience.com/how-to-create-a-photo-mosaic-in-python-45c94f6e8308)
____

**Environment:** 
1. jupyter-notebook
<br>

**Dependencies:**
1. numpy
2. scipy
3. PIL
4. glob
5. matplotlib

**Folds**
* photos store images
* photo/main: main image (only 1 image exist)
* photo/tiles: pixel images

____
**Some solved problems**
1. Using Image.open('path') to open images, some images will not show up with the correct orientation. <br>
_ANS:_ This is because each image has its own orientation information stored in _exif_. That is why I use _ImageOps.exif_transpose() function_ to change its orientation. 
