# Fourier Approximator

The `Elephant.nb` file contains mathematica code for approximating a continuous time function given a bunch of points to interpolate using **fourier transform**.
In particular, it contains a **graphical representation** of what's happening behind the scenes to grasp the physical meaning of the fourier transform, representing all basis function as an **epicycle** in the complex plane.

### Content

The main idea is that given some discrete point, to find a continuous time function interpolating all of them using **fourier theory**.

In this code, you will find out how to compute the continuous time **elephant curve**:

<p align="left" width="100%">
    <img src="https://github.com/user-attachments/assets/6d139e18-de74-4e5a-8e9f-e9fee9221f75">
</p>

The main idea is that we can use **Discrete Fourier Transform** to obtain a continuous function in the frequency domain. The trick now is to sample in the frequency domain and apply the **Inverse Discrete Fourier Transform** to obtain a continuous time periodical function describing a signal interpolating all those points.
Furthermore, we can arbitrarily choice the **precision** of the interpolation by controlling the number of samples in the frequency domain.

### Result

The result shows the continuous time curve describing the elephant. According to fourier theory it can be represented as a **summation of sinusoidal curves**.
In the animation below, it is represented as the summation of all the **epicycles radius of the basis function in the complex plane**. 

<p align="left" width="100%">
    <img src="https://github.com/user-attachments/assets/bbfc625e-5e8c-42a8-9c32-cd028d4121cc">
</p>
