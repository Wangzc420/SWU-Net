# SWU-Net
This is the repository of SWU-Net for complex-valued electrical impedance tomography (Cv-EIT) (submitted to IEEE Signal Processing Letters))

## Introduction
Complex-valued electrical impedance tomography (Cv-EIT) could reconstruct the conductivity and permittivity distributions simultaneously in the observation domain. Whereas, the inverse problem of Cv-EIT is ill-posed and nonlinear resulting the inaccurate admittivities and boundary distortions. In this letter, we propose a novel learning-based image reconstruction method with an ‘end-to-end’ manner to obtain high-quality Cv-EIT image. The two-stage framework is designed to implement manifold transfer and image reconstruction. Specifically, the measured signals are transferred to the initial parameters distribution in the image domain using the iteration-based algorithm. Moreover, a spatial-wavelet dual-domain U-shaped network is proposed, where the low-frequency and high-frequency features are interacted using discrete wavelet transform and convolution/Transformer in the Encoder, bottleneck, and Decoder for conductivity and permittivity fusion. The experimental results show that our method has better performance in terms of quantitative metrics and visual results compared to competing methods. Meanwhile, the ablation study confirms the effectiveness of the spatial-wavelet feature fusion manner.

## Methodology
The overview of SWU-Net is shown as follows.
<div align="center">
  <img src="https://github.com/Wangzc420/SWU-Net/blob/main/Image/Figure1.png">
</div>

The detailed modules of SWU-Net, including Encoder, bottleneck, and Decoder, are given as follows.
<div align="center">
  <img src="https://github.com/Wangzc420/SWU-Net/blob/main/Image/Figure2.png">
</div>

## Experimental set up
The experiment system of EIT-DAS contains contains three parts of a sensor array with 16 electrodes attached on a circle tank, a FPGA-based data acquisition system (DAS), and a host PC for image reconstruction software. The DAS system consists of a sensing array, an FPGA master controller, a digital/analog converter, a voltage-controlled current source (VCCS), a programmable variable gain amplifier (PGA), and a PC software, as shown in Fig. R1. The observation domain is with the radius of 0.19 m, the SNR of this system is about 70 dB, bit resolution of AD converter is 14 bits. The dynamic voltage range of ADC is from −5 V to 5 V. The frequency of excitation current is 50 kHz, and the amplitude of current is 2 mA.

The equipments of DAS and the workflow are shown as:
<div align="center">
  <img src="https://github.com/Wangzc420/SWU-Net/blob/main/Image/Figure3.png">
</div>

## Results

This part gives the simulation results of shape reconstruction and the real-world results of multi-phase and lung-shaped phantom results. The visualizations are given as follows:
<div align="center">
  <img src="https://github.com/Wangzc420/SWU-Net/blob/main/Image/Figure4.png">
</div>

<div align="center">
  <img src="https://github.com/Wangzc420/SWU-Net/blob/main/Image/Figure5.png">
</div>
