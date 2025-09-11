# Estimating-Camera-Pose-from-a-Planar-Object

## Setup
- Open in Google Colab or locally with Jupyter.

## How to Use
1. Run Cells
   - Initial cells will install dependencies, pull needed imports, and pull demo images
2. In the Notebook UI
   - Upload a sample image with the planar scene
   - Upload the intrinsics.json file
   - Use the cursor to select 4 inner corners in the grid
       - Start from either the bottom left or top right corner and move clockwise
           - example:
  
             <img width="418" height="285" alt="image" src="https://github.com/user-attachments/assets/79c339d9-fede-48c0-a60c-476ecb44a756" />


    - To clear the selected corners, choose the **Clear Clicks** option
    - Set pattern size (inner corners) and square size (meters).
    - Click **Estimate Pose**

3. Results
    - Corner Detection: Uses OpenCV's findChessboardCorners
    - Pose from Homography→Pose (R, t).
    - Pose from OpenCV (R, t).
    - Overlay with projected points and axes on the image
    - 3D Plot depicting cameras in the world frame
