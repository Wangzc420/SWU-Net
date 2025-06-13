# SWU-Net
This is the repository of SWU-Net for complex-valued electrical impedance tomography (Cv-EIT) (submitted to IEEE Signal Processing Letters))

## Introduction
Complex-valued electrical impedance tomography (Cv-EIT) could reconstruct the conductivity and permittivity distributions simultaneously in the observation domain. Whereas, the inverse problem of Cv-EIT is ill-posed and nonlinear resulting the inaccurate admittivities and boundary distortions. In this letter, we propose a novel learning-based image reconstruction method with an ‘end-to-end’ manner to obtain high-quality Cv-EIT image. The two-stage framework is designed to implement manifold transfer and image reconstruction. Specifically, the measured signals are transferred to the initial parameters distribution in the image domain using the iteration-based algorithm. Moreover, a spatial-wavelet dual-domain U-shaped network is proposed, where the low-frequency and high-frequency features are interacted using discrete wavelet transform and convolution/Transformer in the Encoder, bottleneck, and Decoder for conductivity and permittivity fusion. The experimental results show that our method has better performance in terms of quantitative metrics and visual results compared to competing methods. Meanwhile, the ablation study confirms the effectiveness of the spatial-wavelet feature fusion manner.

The overview of SWU-Net is shown as follows.
<div align="center">
  <img src="https://github.com/Wangzc420/SWU-Net/blob/main/Image/Figure1.png">
</div>
