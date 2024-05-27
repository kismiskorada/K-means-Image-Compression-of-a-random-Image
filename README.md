# K-means-Image-Compression-of-a-random-Image
In this project, I focused on compressing an image by reducing its color count using K-means clustering, a method known as color quantization. The process simplifies the image's color palette, making the image smaller in file size while sacrificing some detail.
Project Steps:

Image Preparation:

Loaded the image 'parrot.jpg' and converted it to a numerical array.
Reshaped the 3D array (height x width x RGB) into a 2D array where each pixel is a row, and each color channel (R, G, B) is a column.

K-Means Clustering:

Chose 4 as the number of colors to reduce the image to.
Applied K-means clustering, assigning each pixel to the nearest of the 4 centroids and updating centroids based on the average of assigned pixels.

Creating the Quantized Image:

Replaced each pixel's color in the original image with the color of its assigned centroid.
Resulted in a new image with only 4 unique colors.

Results Comparison:

Displayed both original and quantized images side by side.
The original image had a rich color palette, while the quantized version had fewer colors and less detail but was smaller in size.

Compression Analysis:
Original Size: Calculated based on the number of pixels and 8 bits per color channel.
Compressed Size: Used 2 bits per pixel plus storage for the 4 centroids (each 8 bits for R, G, B values).
Compression Rate: Approximately 3.127% of the original size, indicating significant size reduction.

Conclusion:
The K-means quantization effectively reduced the image size by lowering color depth. This approach is beneficial for applications needing reduced storage with acceptable image quality loss. The trade-off between compression and quality is essential in practical uses.

LINK: https://drive.google.com/file/d/1f9hzMtlSIi3sHLy3sqNwqdv7Vpu6ZV57/view?usp=sharing

