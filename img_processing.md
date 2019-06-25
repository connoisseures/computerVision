Image Processing 
===
+ https://askubuntu.com/questions/1091493/convert-a-1-channel-image-to-a-3-channel-image
```python
import cv2
import numpy as np
img = cv2.imread('10524.jpg')
gray = cv2.cvtColor(img, cv2.COLOR_BGR2GRAY)
img2 = np.zeros_like(img)
img2[:,:,0] = gray
img2[:,:,1] = gray
img2[:,:,2] = gray
cv2.imwrite('10524.jpg', img2)
```
### color conversion
+ https://stackoverflow.com/questions/16443553/opencv-python-convert-rgb-to-ycrcb?rq=1 
+ https://docs.opencv.org/3.3.0/de/d25/imgproc_color_conversions.html
+ https://www.learnopencv.com/color-spaces-in-opencv-cpp-python/
+ https://stackoverflow.com/questions/48125095/convert-rgb-image-to-yuv-and-ycbcr-color-space-image-in-opencv-python
