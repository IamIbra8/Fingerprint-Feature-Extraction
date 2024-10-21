# Fingerprint-Feature-Extraction
This is a project which uses the fundamentals of Image Processing to extract the features (edges and ridges) from a fingerprint's image.

Fingerprint biometrics involve: Image Acquisition, Image Enhancing, Feature extraction and matching with template. Since the dataset has unique fingerprints I will implement feature extraction and different techniques for enhancing images such as Edge detection, adaptive thresholding. Feature extraction constitutes of Ridge detection (level 1 feature) and Minutiae extraction (level 3 feature) to generate a template after whicha query image is matched using the metric ROC AUC curve.
I have used Image enhancement and preprocessing techniques such as smoothing, thresholding and edge detection are used to make features more prominent in data for extraction to be more accurate, applied Robert, Sobel and Prewitt filter.
Lastly, to show the results clearly, I have used these functions:
  1) getTerminationBifurcation: This function takes the skeletonized fingerprint image and its corresponding mask as input. It identifies minutiae points (terminations and bifurcations) based on the local pattern of the skeletonized image. It returns binary images marking the locations of terminations and bifurcations.
  2) ShowResults: This function visualizes the extracted minutiae features on the skeletonized image. It overlays circles on the image to represent the locations of terminations (in blue) and bifurcations (in red). It also prints the coordinates and types of each minutiae point.
