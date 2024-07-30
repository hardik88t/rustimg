# Rustimg

Rustimg is a Rust project that processes images using FFmpeg. It automates the generation of image variants with various dimensions and file sizes, ensuring proper naming and organization.

## Features

- **Image Cropping**: For non-square images, Rustimg generates 2 to 8 random square cuts, including a centered cut and additional random positions. Sizes include 100px, 250px, 500px, 1000px, and 1444px.
- **Image Resizing**: Resizes square images to variants of 100kb, 250kb, 500kb, 800kb, 1Mb, and 2Mb, if the resized image is smaller than the original.

## Usage

1. **Place Images**: Put all images in the specified folder.
2. **Run Rustimg**: Execute the Rustimg application to process the images.
3. **Check Output**: The images will be cropped and resized with appropriate names, e.g., `img_800px.png` or `img_800px_100kb.png`.

## Naming Convention

- Cropped images: `originalname_size.png` (e.g., `img_800px.png`)
- Resized images: `originalname_size_filesize.png` (e.g., `img_800px_100kb.png`)

## Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/hardik88t/rustimg.git
