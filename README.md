#JPEG Compression for Color Image
This MATLAB program performs JPEG compression on a color image. The program converts the image to the YCbCr color space, applies downsampling, performs Discrete Cosine Transform (DCT) on 8x8 blocks, quantizes the DCT coefficients, and finally uses Huffman coding to compress the image. The result is displayed alongside the original image to show the effects of compression.

#Files
JPEGCompression.m: Main MATLAB script for JPEG compression.
peppers.png: Sample image used for compression. You can replace it with your own images.
#How to Use
Clone the repository or download the files.
Open JPEGCompression.m in MATLAB.
Ensure you have the Image Processing Toolbox installed.
Run the script. The original and compressed images will be displayed, and the compression ratio will be printed to the console.
#Dependencies
MATLAB (R2019b or later)
Image Processing Toolbox
