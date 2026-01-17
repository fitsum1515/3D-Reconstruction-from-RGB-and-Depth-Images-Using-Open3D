# 3D Reconstruction from RGB and GrayScale Depth Images 
This project implements a 3D reconstruction pipeline that converts a 2D RGB image and its corresponding depth image into a 3D colored point cloud and a triangular mesh using Python and the Open3D library. The system demonstrates fundamenta techniques in computer vision, robotics perception, and intelligent systems.
# 📌 Project Overview
Give:
- An **RGB image** (baby.jpeg) containing color and texture information, and
- A **grayscale depth image**(image.png) encoding per-pixel depth values,

  the system:
  1. Converts the depth image into 3D coordinates using camera intrinsic parameters,
  2. Fuses RGB color information with 3D points,
  3. Constructs a surface mesh using pixel connectivity
  4. Visualizes both the point cloud and the reconstructed mesh.
  # 📂 Project Structure
  
  |── Project_2.py............................ Main reconstruction script
  
  |── baby.jpeg .............................. RGB input image
  
  |── image.png .............................. Grayscale depth range image
  
  |── README.md .............................. Project documentation

  # 🔧 Requirements
  - Python 3.8+
  - Open3D
  - Numpy
 
    # 🚀 How to Run
    1. Place baby.jpeg and image.png in the same directory as as project_2.py.
    2. 
