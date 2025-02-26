# ANPR
 Introduction:
 The Automatic Number Plate Recognition (ANPR) system is a computer vision-based
 technology designed to extract and recognize license plate information from images or
 videos of vehicles. This project aims to develop an ANPR system using OpenCV,
 EasyOCR, and Python to detect and recognize license plates from images.
 Methodology
 The ANPR system consists of the following stages:
 1. Image Preprocessing: The input image is converted to grayscale to simplify
 processing and reduce computational complexity.
 2. Edge Detection: The Canny edge detection algorithm is applied to the grayscale
 image to extract important features like boundaries and shapes.
 3. Contour Detection: The contours of the image are detected using the
 cv2.findContours function, and the contours are sorted based on their areas.
 4. Shape Detection: The contours are approximated using the Douglas-Peucker
 algorithm to simplify the shape, and quadrilaterals (four-sided shapes) are
 identified as potential license plates.
 5. Masking: A mask is created to isolate the detected license plate region from the
 rest of the image.
 6. Bitwise AND Operation: The original image is combined with the mask using a
 bitwise AND operation to extract the license plate region.
 7. Cropping: The license plate region is cropped from the original image.
8. Optical Character Recognition (OCR): The EasyOCR library is used to recognize
 the text on the license plate.
 9. Result Display: The recognized text is displayed on the original image along with
 a bounding box around the license plate.
 The following libraries are used in this project:
 OpenCV
 OpenCV is a computer vision library that provides a wide range of functions for image
 and video processing, feature detection, object recognition, and more. In this project,
 OpenCV is used for:
 ● Imagereading and writing
 ● Grayscale conversion
 ● Edgedetection (Canny algorithm)
 ● Contour detection
 ● Shapeapproximation (Douglas-Peucker algorithm)
 ● Masking and bitwise AND operation
 ● Drawing contours and bounding boxes
 Imutils
 Imutils is a library that provides a set of convenience functions for working with OpenCV.
 In this project, Imutils is used for:
 ● Grabbing contours from the cv2.findContours function
 EasyOCR
 EasyOCR is a Python library that provides an easy-to-use interface for optical character
 recognition (OCR). In this project, EasyOCR is used for:
● Recognizing text on the license plate
 Implementation
 The implementation of the ANPR system involves the following steps:
 1. Read the input image using OpenCV.
 2. Convert the image to grayscale using cv2.cvtColor.
 3. Apply the Canny edge detection algorithm using cv2.Canny.
 4. Detect contours using cv2.findContours and sort them based on their areas.
 5. Approximate the contours using the Douglas-Peucker algorithm and identify
 quadrilaterals.
 6. Create a mask to isolate the detected license plate region.
 7. Perform a bitwise AND operation to extract the license plate region.
 8. Crop the license plate region from the original image.
 9. Use EasyOCR to recognize the text on the license plate.
 10.Display the recognized text on the original image along with a bounding box
 around the license plate.
 Results
 The ANPR system is able to successfully detect and recognize license plates from
 images. The system is able to handle various types of license plates, including those
 with different fonts, colors, and orientations.
Conclusion:
 The ANPR system developed in this project demonstrates the potential of computer
 vision and OCR techniques in extracting and recognizing license plate information from
 images. The system can be further improved by incorporating additional features, such
 as image enhancement, noise reduction, and more advanced OCR algorithms. The
 ANPR system has various applications in traffic monitoring, law enforcement, and
 intelligent transportation systems
