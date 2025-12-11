# 🚀 Image Upscaler AI

**Transform low-resolution images into high-quality visuals using state-of-the-art AI models.**

![Project Demo](Screenshot%202025-12-12%20031526.png)

## 📖 About

Image Upscaler AI is a powerful, easy-to-use image enhancement tool that runs entirely in Google Colab. Leveraging **Real-ESRGAN** for super-resolution and **GFPGAN** for face restoration, this project enables anyone to upscale and enhance images up to **4x resolution** with professional-grade results—no technical expertise required.

Whether you're a photographer, designer, content creator, or anyone looking to enhance low-resolution images, this tool provides an intuitive Gradio-based web interface for seamless image processing.

## ✨ Features

- 🔍 **2x & 4x Upscaling** - Enhance image resolution with Real-ESRGAN
- 🎭 **Face Enhancement** - Restore and improve facial details with GFPGAN
- 🖼️ **Interactive UI** - User-friendly Gradio web interface
- 📊 **Comparison View** - Side-by-side before/after visualization
- 🗂️ **Batch Processing** - Process multiple images at once
- ⚡ **GPU Accelerated** - Fast processing with CUDA support (T4 GPU in Colab)
- 💾 **High Quality Output** - Preserves image quality and details
- 🌐 **Public Sharing** - Share your results with a public URL

## 🛠️ Tech Stack

- **Framework**: Python 3.x
- **Deep Learning**: PyTorch
- **Super-Resolution**: Real-ESRGAN (xinntao)
- **Face Enhancement**: GFPGAN (TencentARC)
- **Web Interface**: Gradio
- **Image Processing**: OpenCV, PIL, NumPy
- **Environment**: Google Colab (Free GPU - T4)

## 📋 Requirements

No local installation needed! This notebook runs entirely in Google Colab with:
- Google account (Free)
- Internet connection
- ~5 minutes for initial setup

## 🚀 Quick Start Guide

### Step 1: Open in Google Colab

Click the badge to open the notebook:

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/adityapawar327/DetailBoost-AI/blob/main/Image_Upscaler_AI.ipynb)

### Step 2: Enable GPU

1. Click **Runtime** → **Change runtime type**
2. Select **T4 GPU** as Hardware accelerator
3. Click **Save**

### Step 3: Run All Cells

1. Go to **Runtime** → **Run all**
2. Wait 3-5 minutes for installation
3. When prompted, click **"Restart Runtime"** (around Cell 2)
4. After restart, **Run all cells again**

### Step 4: Wait for Gradio Link

1. Scroll to the last cell output
2. Wait for the **public URL** to appear
3. Look for: `Running on public URL: https://...`

### Step 5: Upscale Your Image

1. **Upload** your image
2. **Select** upscale factor (2x or 4x)
3. **Enable** face enhancement (optional)
4. **Click** "Upscale Image" button
5. **Download** your result

## 📊 Processing Details

| Feature | 2x Upscale | 4x Upscale | Face Enhancement |
|---------|-----------|-----------|------------------|
| Speed | Fast (5-10s) | Medium (15-30s) | Slower (20-40s) |
| Quality | Good | Excellent | Best for faces |
| Use Case | Quick previews | Final output | Portraits/Selfies |

## 🎯 Use Cases

✅ **Photo Restoration** - Enhance old, faded photographs
✅ **Old Screenshots** - Upscale low-res game captures
✅ **Social Media Content** - Improve image quality
✅ **Portrait Enhancement** - Restore facial details
✅ **Web Images** - Enlarge web-sourced images
✅ **Design Assets** - Scale up graphics
✅ **Gaming Content** - Enhance gameplay screenshots
✅ **Content Creation** - Prepare high-quality images for videos

## 📚 How It Works

### Real-ESRGAN (Super-Resolution)

Real-ESRGAN is a state-of-the-art GAN-based model trained on millions of images to:
- Remove noise while upscaling
- Preserve fine details and textures
- Handle 2x and 4x scaling factors
- Work with diverse image types

### GFPGAN (Face Enhancement)

GFPGAN is specialized for face restoration that:
- Detects and enhances facial features
- Restores skin texture and details
- Improves eyes, nose, and mouth clarity
- Works with realistic and artistic faces

## 🟶️ Interface Overview

**Left Panel (Input)**:
- Image upload area
- Upscale factor selection
- Face enhancement toggle
- Comparison view option
- Processing button

**Right Panel (Output)**:
- Upscaled result or comparison
- Processing statistics
- Before/after dimensions
- Quality metrics

## ⚒️ Advanced Usage

### Batch Processing

1. Upload images one by one
2. Wait for each to complete
3. Download results

### Comparison Mode

Enable "Show Side-by-Side Comparison" to:
- View original and upscaled together
- Better assess improvement
- Share before/after visuals

## 🔧 Troubleshooting

### CUDA Out of Memory Error
- Reduce image size before uploading
- Use 2x upscale instead of 4x
- Reduce the `tile` parameter

### Models Not Downloading
- Check internet connection
- Ensure free space on Colab
- Restart runtime and try again

### Gradio Link Not Appearing
- Scroll down to see latest output
- Wait 30 seconds after "Loading models"
- Check for errors in previous cells

## 📋 Model Information

**RealESRGAN_x4plus**: ~170MB, trained for robust upscaling, Apache 2.0
**RealESRGAN_x2plus**: ~170MB, optimized for 2x upscaling, Apache 2.0
**GFPGANv1.3**: ~350MB, specialized for face restoration, Apache 2.0

## 💫 Tips for Best Results

1. Higher input quality = better results
2. Use PNG or JPEG formats
3. Works best with images up to ~4000x4000 pixels
4. Keep faces clearly visible for face enhancement
5. First load takes longer, subsequent runs are faster
6. Share results using the public URL

## 🚫 Limitations

- Cannot create genuine new information
- Extremely low-res images (<50x50px) may not work well
- Face enhancement works best with clear frontal faces
- Processing time varies with image size and GPU
- Public URLs expire after 72 hours

## 🔐 Privacy & Data

- Images processed locally on Colab's GPU
- No images stored after processing
- No external server transmission
- Your notebook is private

## 📬 License

- Real-ESRGAN: Apache License 2.0
- GFPGAN: Apache License 2.0
- Gradio: Apache License 2.0
- PyTorch: BSD License

## 🌟 Credits

- Real-ESRGAN by Xintao Wang (TencentARC)
- GFPGAN by Xintao Wang (TencentARC)
- Gradio by Hugging Face
- PyTorch by Facebook AI Research

---

**Made with ❤️ using AI for creative enhancement**

*Last Updated: December 12, 2025*
