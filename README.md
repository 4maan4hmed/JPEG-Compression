# 📷 JPEG Compression for Color Images

## 📌 Overview
This MATLAB project demonstrates **JPEG compression** on a color image, breaking down the standard JPEG pipeline into key steps: **color space conversion, downsampling, Discrete Cosine Transform (DCT), quantization, entropy encoding, and Huffman coding**. The output showcases the trade-offs between image quality and file size.

## 🔍 Features
- **Supports any RGB image** (e.g., `.png`, `.jpg`)
- **YCbCr Color Space Conversion** for better compression
- **Chroma Subsampling (4:2:0)** to reduce data size
- **8x8 DCT Transform and Quantization** to eliminate visual redundancies
- **Huffman Encoding** for efficient compression
- **Adjustable Compression Levels** to analyze quality loss vs. compression ratio

## 📂 Files Included
- `jpeg_compression.m` → Main MATLAB script for JPEG compression
- `peppers.png` → Sample image for compression (replaceable with your own image)
- `quantization_tables.mat` → Contains predefined quantization matrices

## 🚀 How to Use
1. **Clone or Download** this repository.
2. **Open `jpeg_compression.m`** in MATLAB.
3. **Ensure you have the Image Processing Toolbox installed.**
4. **Run the script.** It will:
   - Convert the image to YCbCr
   - Apply chroma subsampling
   - Perform 8x8 DCT and quantization
   - Encode the image with Huffman coding
   - Display and compare compressed images

## 📊 Compression Levels
The script generates output images at different compression levels to compare quality loss:

| Compression Quality | Description |
|---------------------|-------------|
| **High (Q=90)** | Near-lossless compression with minimal artifacts |
| **Medium (Q=50)** | Good balance between quality and file size |
| **Low (Q=10)** | High compression with visible artifacts |

## 📷 Sample Results
Below are images demonstrating different compression levels:

1. **Compressed Image 1 (High Quality)**<br>
   ![Original Image](https://github.com/4maan4hmed/JPEG-Compression/blob/main/Compressed%20Image%201.png)

2. **Compressed Image 2 (High Quality)**<br>
   ![High Quality](https://github.com/4maan4hmed/JPEG-Compression/blob/main/Compressed%20Image%202.png)

3. **Compressed Image 2 (Low Quality)**<br>
   ![Medium Quality](https://github.com/4maan4hmed/JPEG-Compression/blob/main/Highly%20Compresed%20Image%202.jpg)

## 🛠 Dependencies
- **MATLAB R2019b or later**
- **Image Processing Toolbox** (for color space conversion and image handling)

## 🔧 Customization
You can adjust the **quantization matrix** and **chroma subsampling** in `jpeg_compression.m` to experiment with different compression effects.

## ⚠️ Known Limitations
- **Does not implement progressive JPEG compression**
- **Limited to 8-bit images (24-bit RGB)**
- **Huffman coding does not use an adaptive dictionary**

## 📚 Further Reading
For an in-depth understanding of JPEG compression:
- [JPEG Standard (ITU-T.81)](https://www.w3.org/Graphics/JPEG/itu-t81.pdf)
- MATLAB’s built-in `imwrite` function for JPEG
- Image Compression concepts: https://en.wikipedia.org/wiki/JPEG

---
🔬 *This project is meant for educational purposes to understand the JPEG compression pipeline. It is not optimized for real-world large-scale image compression.*

