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
    2. Update the file inside Project_2.py     
    3. Run the script: project_2.py     
    4. Two windows will appear:
       - A 3D colored point cloud
       - A 3D triangular mesh
      
     # 🧠 Methodology

## 1.  Depth Image Processing

   The grayscale depth image is converted into metric depth values and filtered to remove invalid pixels.

## 2.  3D projection

   Each pixel is projected into 3D space using the pinhole camera model:

Where:
- u, v are pixel coordinates,
- d is the depth value,
- fx, fy, cx, cy are camera intrinsic parameters.

## 3.  Color Fusion

  RGB values from baby.jpeg are assigned to each 3D point, creating a colored point cloud.

## 4. Mesh Generation

  Neighboring depth pixels are triangulated to form a surface mesh, followed by mesh cleanup to remove degenerate and non-manifold elements.

  # 🎯 Applications
  - Robotics perception
  - COmputer vision and 3D modeling
  - Digital design and fabrication
  - SMart systems and Intelligent environments
  - Simulation and visualization

  # 📸 Input
  - RGB Image : baby.jpeg
  - Depth Image : image.png (grayscale depth range)
  # 🛠️ Future Improvements
  - Add real-time depth acqisition from RGB-D cameras
  - Implement noise filtering and depth smoothing
  - Integrating deep learning-based depth estimation
  - Export mesh for 3D printing (STL/OBJ)
  - Add quantitative reconstruction accuracy evaluation







  
   









    
