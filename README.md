## Computer Vision Tutorial

_Computer Vision Tutorial_ includes classical theories and techniques and also recent ML/DL-based methods for computer vision. As classical theories and techniques, the tutorial contains image processing, camera projection models, camera calibration, and pose estimation. As recent ML/DL-based methods, the tutorial deals with object categorization (and backbone networks), and its extensions such as object detection and instance segmentation. It also explains about further topics such as multi-object tracking, structure-from-motion, NeRF, and so on.

This tutorial has been initiated and maintained to teach undergraduate CSE students in [SEOULTECH](https://en.seoultech.ac.kr/) as the course of _Computer Vision_ (109079).

This tutorial contains code examples briefly written in [Python](https://python.org/) with [OpenCV](https://opencv.org/) and [PyTorch](https://pytorch.org/).
* :bulb: Some of codes will help readers to understand **inside** of algorithms (e.g. how it works).
* :wrench: The others of codes will provide **usages and applications** of OpenCV functions (e.g. how to use it).



### Lecture Slides
* [Section 1. Introduction](https://github.com/mint-lab/cv_tutorial/blob/master/slides/01_introduction.pdf)
* [Section 2. Image Editing: Learning OpenCV](https://github.com/mint-lab/cv_tutorial/blob/master/slides/02_image_editing.pdf)
* [Section 3. Image Processing](https://github.com/mint-lab/cv_tutorial/blob/master/slides/03_image_processing.pdf)
* [Section 4. Image Formation](https://github.com/mint-lab/cv_tutorial/blob/master/slides/04_image_formation.pdf)
* [Section 5. Color](https://github.com/mint-lab/cv_tutorial/blob/master/slides/05_color.pdf)
* [Section 6. Image Geometry](https://github.com/mint-lab/cv_tutorial/blob/master/slides/06_image_geometry.pdf)
* [Section 7. Visual Features](https://github.com/mint-lab/cv_tutorial/blob/master/slides/07_visual_features.pdf)
* [Advanced Topic 1. How to Solve Equations](https://github.com/mint-lab/cv_tutorial/blob/master/slides/adv01_solving_equations.pdf)



### Example Codes
* **Section 1. Introduction** [(Slides)](https://github.com/mint-lab/cv_tutorial/blob/master/slides/01_introduction.pdf)
   * Note) How to install prerequisite packages in Python: `pip install -r requirements.txt`
* **Section 2. Image Editing: Learning OpenCV** [(Slides)](https://github.com/mint-lab/cv_tutorial/blob/master/slides/02_image_editing.pdf)
   * OpenCV Image Representation
      * Image creation: [image_creation.py](https://github.com/mint-lab/cv_tutorial/blob/master/examples/image_creation.py) :bulb:
   * OpenCV Image and Video Input/Output
      * Image file viewer: [image_viewer.py](https://github.com/mint-lab/cv_tutorial/blob/master/examples/image_viewer.py) :wrench:
      * Image format converter: [image_converter.py](https://github.com/mint-lab/cv_tutorial/blob/master/examples/image_converter.py) :wrench:
      * Video file player: [video_player.py](https://github.com/mint-lab/cv_tutorial/blob/master/examples/video_player.py) :wrench:
      * Video format converter: [video_converter.py](https://github.com/mint-lab/cv_tutorial/blob/master/examples/video_converter.py) :wrench:
   * OpenCV Drawing Functions
      * Shape drawing: [shape_drawing.py](https://github.com/mint-lab/cv_tutorial/blob/master/examples/shape_drawing.py) :wrench:
   * OpenCV High-level GUI
      * (Handling keyboard events) Video file player with frame navigation: [video_player+navigation.py](https://github.com/mint-lab/cv_tutorial/blob/master/examples/video_player%2Bnavigation.py) :wrench:
      * (Handling mouse events) Free drawing: [free_drawing.py](https://github.com/mint-lab/cv_tutorial/blob/master/examples/free_drawing.py) :wrench:
   * Image Editing
      * Negative image and flip: [negative_image_and_flip.py](https://github.com/mint-lab/cv_tutorial/blob/master/examples/negative_image_and_flip.py) :bulb:
      * Intensity transformation with contrast and brightness: [intensity_transformation.py](https://github.com/mint-lab/cv_tutorial/blob/master/examples/intensity_transformation.py) :bulb:
      * (Image addition) Alpha blending: [alpha_blending.py](https://github.com/mint-lab/cv_tutorial/blob/master/examples/alpha_blending.py) :bulb:
      * (Image addition) Background extraction: [background_extraction.py](https://github.com/mint-lab/cv_tutorial/blob/master/examples/background_extraction.py) :bulb:
      * (Image subtraction) Image difference: [image_difference.py](https://github.com/mint-lab/cv_tutorial/blob/master/examples/image_difference.py) :bulb:
      * (Image subtraction) Background subtraction: [background_subtraction.py](https://github.com/mint-lab/cv_tutorial/blob/master/examples/background_subtraction.py) :bulb:
      * (Image crop) Image file viewer with the zoom window: [image_viewer+zoom.py](https://github.com/mint-lab/cv_tutorial/blob/master/examples/image_viewer%2Bzoom.py) :bulb:
      * Image resize with backward value copy: [image_resize.py](https://github.com/mint-lab/cv_tutorial/blob/master/examples/image_resize.py) :bulb:
      * Image rotation with backward/forward value copy: [image_rotation.py](https://github.com/mint-lab/cv_tutorial/blob/master/examples/image_rotation.py) :bulb:
* **Section 3. Image Processing** [(Slides)](https://github.com/mint-lab/cv_tutorial/blob/master/slides/03_image_processing.pdf)
   * Intensity Transformation
     * Image histogram: [histogram.py](https://github.com/mint-lab/cv_tutorial/blob/master/examples/histogram.py) :bulb:
     * Contrast stretching with min-max stretching: [contrast_stretching.py](https://github.com/mint-lab/cv_tutorial/blob/master/examples/contrast_stretching.py) :bulb:
     * Histogram equalization: [histogram_equalization.py](https://github.com/mint-lab/cv_tutorial/blob/master/examples/histogram_equalization.py) :wrench:
   * Thresholding: [thresholding.py](https://github.com/mint-lab/cv_tutorial/blob/master/examples/thresholding.py) :wrench:
   * Image Filtering
     * Image filtering with various kernels: [image_filtering.py](https://github.com/mint-lab/cv_tutorial/blob/master/examples/image_filtering.py) :bulb:
     * Median filter: [median_filter.py](https://github.com/mint-lab/cv_tutorial/blob/master/examples/median_filter.py) :wrench:
     * Sobel edge detection: [Sobel_edge.py](https://github.com/mint-lab/cv_tutorial/blob/master/examples/Sobel_edge.py) :bulb:
     * Canny edge detection: [Canny_edge.py](https://github.com/mint-lab/cv_tutorial/blob/master/examples/Canny_edge.py) :wrench:
     * Bilateral filter: [bilateral_filter.py](https://github.com/mint-lab/cv_tutorial/blob/master/examples/bilateral_filter.py) :wrench:
   * Morphological Operations
     * Morphological operations with various operations and kernels: [morpology.py](https://github.com/mint-lab/cv_tutorial/blob/master/examples/morpology.py) :wrench:
     * Application) Background subtraction (foreground extraction): [background_subtraction.py](https://github.com/mint-lab/cv_tutorial/blob/master/examples/background_subtraction.py) :wrench:
* **Section 4. Image Formation** [(Slides)](https://github.com/mint-lab/cv_tutorial/blob/master/slides/04_image_formation.pdf)
   * Note) 3D rotation conversion: [3d_rotation_conversion.py](https://github.com/mint-lab/cv_tutorial/blob/master/examples/3d_rotation_conversion.py) :wrench:
   * Camera Projection Models
     * Object localization: [object_localization.py](https://github.com/mint-lab/cv_tutorial/blob/master/examples/object_localization.py) :bulb:
     * Image formation: [image_formation.py](https://github.com/mint-lab/cv_tutorial/blob/master/examples/image_formation.py) :bulb:
     * Distortion visualization: [distortion_visualization.py](https://github.com/mint-lab/cv_tutorial/blob/master/examples/distortion_visualization.py) :bulb:
     * Distortion correction: [distortion_correction.py](https://github.com/mint-lab/cv_tutorial/blob/master/examples/distortion_correction.py) :wrench:
   * Camera calibration with a chessboard: [camera_calibration.py](https://github.com/mint-lab/cv_tutorial/blob/master/examples/camera_calibration.py) :wrench:
   * Camera pose estimation with a chessboard: [pose_estimation_chessboard.py](https://github.com/mint-lab/cv_tutorial/blob/master/examples/pose_estimation_chessboard.py) :wrench:
* **Section 5. Color** [(Slides)](https://github.com/mint-lab/cv_tutorial/blob/master/slides/05_color.pdf)
  * Color space conversion: [color_bgr2hsv.py](https://github.com/mint-lab/cv_tutorial/blob/master/examples/color_bgr2hsv.py) :wrench:
  * Color histogram equalization: [histogram_equalization+color.py](https://github.com/mint-lab/cv_tutorial/blob/master/examples/histogram_equalization+color.py) :bulb:
* **Section 6. Image Geometry** [(Slides)](https://github.com/mint-lab/cv_tutorial/blob/master/slides/06_image_geometry.pdf)
   * Camera pose estimation with a book cover v1: [pose_estimation_book1.py](https://github.com/mint-lab/cv_tutorial/blob/master/examples/pose_estimation_book1.py) :wrench:
   * Perspective correction: [perspective_correction.py](https://github.com/mint-lab/cv_tutorial/blob/master/examples/perspective_correction.py) :wrench:
   * Image stitching: [image_stitching.py](https://github.com/mint-lab/cv_tutorial/blob/master/examples/image_stitching.py) :wrench:
   * 2D video stabilization: [video_stabilization.py](https://github.com/mint-lab/cv_tutorial/blob/master/examples/video_stabilization.py) :wrench:
   * Triangulation: [triangulation.py](https://github.com/mint-lab/cv_tutorial/blob/master/examples/triangulation.py) :wrench:
* **Section 7. Visual Features** [(Slides)](https://github.com/mint-lab/cv_tutorial/blob/master/slides/07_visual_features.pdf)
* **Section 8. Object Recognition**
* **Section 9. Object Tracking**
* **Advanced Topics 1. How to Solve Equations** [(Slides)](https://github.com/mint-lab/cv_tutorial/blob/master/slides/adv01_solving_equations.pdf)
   * Solving inhomogeneous linear equations
      * Affine transformation estimation: [affine_estimation.py](https://github.com/mint-lab/cv_tutorial/blob/master/examples/affine_estimation.py) :bulb:
   * Solving homogeneous linear equations
      * Planar homography estimation: [homography_estimation.py](https://github.com/mint-lab/cv_tutorial/blob/master/examples/homography_estimation.py) :bulb:
         * Note) Image warping: [image_warping.py](https://github.com/mint-lab/cv_tutorial/blob/master/examples/image_warping.py) :bulb:
      * Triangulation: [triangulation_implement.py](https://github.com/mint-lab/cv_tutorial/blob/master/examples/triangulation_implement.py) :bulb:
   * Solving nonlinear equations
      * Camera pose estimation (PnP): [pose_estimation_implement.py](https://github.com/mint-lab/cv_tutorial/blob/master/examples/pose_estimation_implement.py) :bulb:
      * Camera calibration: [camera_calibration_implement.py](https://github.com/mint-lab/cv_tutorial/blob/master/examples/camera_calibration_implement.py) :bulb:




### Authors
* [Sunglok Choi](https://github.com/sunglok)



### Acknowledgements
The authors thank the following contributors and projects.

* [ImageProcessingPlace.com](https://www.imageprocessingplace.com/root_files_V3/image_databases.htm) for test images (`lena.tif`, `baboon.tif`, and `peppers.tif`)
* [MOTChallenge](https://motchallenge.net/vis/PETS09-S2L1) for test images (`PETS09-S2L1-raw.webm`)
* [Wikipedia](https://en.wikipedia.org/wiki/Salt-and-pepper_noise) for a test image (`salt_and_pepper.png`)
* [OpenCV](https://github.com/opencv/opencv/tree/4.x/samples/data) for a test image (`sudoku.png`)
