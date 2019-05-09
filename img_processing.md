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
  + 
