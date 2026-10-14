# Digital-Image-Processing-Project
Provides an algorithmic exploration of foundational Digital Image Processing (DIP) techniques. This project implements and benchmarks low-level spatial and frequency-domain operations from mathematical first principles—including manual sliding-window spatial convolutions, non-linear median reduction as well as 4-connected boundary discovery


## Key Features

- **Multi-Color Space Analysis**: Channel decomposition across Cartesian (RGB) and cylindrical (HSV) coordinate models to evaluate chroma/luma variance.
- **Dynamic Binarization & Statistical Modeling**: Normalized grayscale projection coupled with adaptive threshold estimation (Otsu's criterion) and global histogram analysis.
- **Affine & Morphological Transformations**: Resolution scaling via anti-aliasing interpolation, geometric fixed-frame re-projection ($250 \times 250$), and orthogonal 2D matrix rotations.
- **Stochastic Degradation Simulation**: Zero-mean additive Gaussian white noise injection ($\sigma = 45$) modeling real-world sensor noise.
- **From-Scratch Non-Linear Filtering**: Pure vector/array-level $5 \times 5$ median filter implementation avoiding high-level library abstractions (`scipy.ndimage`, `cv2.medianBlur`).
- **Topological Boundary Detection**: 4-neighborhood contour extraction algorithm for spatial boundary discovery on discretized grids.
- **Frequency-Domain Signal Processing**: 2D Fast Fourier Transform (FFT) manipulation combined with an $n$-th order low-pass Butterworth transfer function for continuous frequency attenuation.
- **Spatial Gradient Operators**: Discrete directional edge approximation using separable horizontal and vertical $3 \times 3$ Sobel convolution kernels.
