# Picture-Cartoon
This project uses OpenCV library in Python to convert a given picture into a cartoon-like image. The process involves applying different image processing techniques such as bilateral filtering, edge detection, and color quantization to the input image.

This process can be broken down into several steps:

Loading the image: The first step is to load the input image using OpenCV's imread() function.

Applying bilateral filtering: Bilateral filtering is a technique used to smooth an image while preserving its edges. This is important for creating cartoon-like images as we want to preserve the edges of the objects in the image. The bilateralFilter() function in OpenCV can be used to apply this filter to the image.

Detecting edges: The next step is to detect the edges in the image using the Canny edge detector. This will help us identify the boundaries between objects in the image. The Canny() function in OpenCV can be used to apply this filter to the image.

Applying color quantization: Color quantization is a technique used to reduce the number of colors in an image. This can help give the image a cartoon-like appearance. The kmeans() function in OpenCV can be used to cluster the colors in the image and assign each pixel to a color cluster.

Combining the results: Finally, we can combine the results of the bilateral filtering, edge detection, and color quantization to create the final cartoon-like image. This can be done by multiplying the edges image with the color quantized image.

Once these steps are complete, the resulting image should have a cartoon-like appearance with strong edges and reduced colors. The exact parameters used for each step will depend on the input image and the desired output, so it may require some experimentation to find the optimal settings.

Overall, this project is a great way to learn about image processing techniques and how they can be used to create interesting visual effects.
