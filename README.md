Image Stitching 
========================
By: Pavan Kumar 

## Summary
OpenCV and Python program to stitch two input images.

## Usage Instructions
- Use the command
```
python stitch_images.py <FirstImage> <SecondImage>
```
- Output images will be written inside the folder 'results'

---

The code was modified to make the program able to run.

1. module ‘cv2’ has no attribute ‘SIFT’ ：The reason for the version change
   
In the new version, OpenCV has integrated algorithms such as SIFT into the xfeatures2d module.

```
# Initialize SIFT 
# sift = cv2.SIFT()
sift=cv2.xfeatures2d.SIFT_create()
```

2. Support python3.x 

```print('Error: Not enough matches')```

3. 运行

```$ python stitch_images.py images/01_suburbA.jpg images/01_suburbB.jpg```

参考：

https://github.com/pavanpn/Image-Stitching

https://blog.csdn.net/Nismilesucc/article/details/111240945