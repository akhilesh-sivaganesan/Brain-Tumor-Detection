# Brain Tumor Detector
Given CT scan, identify if the scan contains a brain tumor. This project is outlined by 5 steps: data input, preprocessing steps, classification algorithm architecture, and the results.
## (1) Data Input
The data input consists of 1000 CT scans, 500 of which contain brain tumors and the remaining 500 that do not contain tumors. These 1000 images were used to train a convolutional neural network.
## (2) Preprocessing
Two main steps were taken to preprocess and simplify the output of the data and reduce the training/run time of the algorithm.
### Varying sizes of CT scans
Using Matplotlib, the maximum size of the images was found and all CT scans were superimposed onto a canvas of that size. This way, the CT scan size is standardized. 
### Varying color of CT scan
The colors were removed from the CT scan as sources had varying colors. Removal of the RGB layer enabled the usage of only the black/white layer of the image to further simplify the input for the algorithm.
## (3) Classification Algorithm
Evaluated varying performance of CNN, KNN, and RNN architectures in tumor detection
## (4) Results
Discovered KNN performed best with 84.1% true positive & 72.7% of true negative accuracy.

## (5) Future Improvements
Evaluate the layers of the KNN architecture and determine which activation functions and training/validation splits work optimally. Furthermore, investigate a neural network that can handle varying image sizes and colors as important information may have been lost in the simplification process.
