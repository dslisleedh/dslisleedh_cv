<h1>
<div align="center">
  이동헌(Dongheon Lee, dslisleedh)
</div>
</h1>

<div align="right">
  <b>Birth:</b> 12/22/1997 
  
  <b>Phone:</b> +82-10-2998-5715  
  
  <b>Email:</b> dslisleedh@gmail.com
</div>

## Career  
 - UST21 (Research & Development department)
   - AI Engineer (Mar. 2022 ~ Apr. 2023)  
   - Work experiences  
     - <b>Sea-Surface-Temperature super resolution</b> (July 2022 ~ Apr. 2023)  
       ![SST_SR_result](https://github.com/dslisleedh/dslisleedh_cv/blob/main/sst_sr_result.PNG)
       To upscale SST data from remote sensing, I tested two strategies: SISR and MISR. I chose NAFSR (Non-linear Activate Free Network for Super-Resolution) for SISR because of its simplicity, and TR-MISR for MISR because it is the SOTA model in the unique MISR dataset, PROBA-V. SISR (NAFSR) performed best, with a PSNR gain of +0.97 dB over MISR and +1.34 dB over bicubic interpolation at scale 4. 
       
     - <b>Sea-fog generation prediction</b> (Apr. 2022 ~ Dec. 2022)  
        I tested various models to handle an extremely imbalanced time-series classification dataset. After the training is complete, I deploy the model to the actual service. [[Link]](http://www.khoa.go.kr/oceanmap/pois/popup_seafog.do?lang=ko)  
        Models tested:
          - Transformer
          - GFNet
          - 1D-Convolution based model

     - <b>Anomaly detection on maritime AIS data</b> (May 2022 ~ Nov. 2022)  
       ![Model](https://github.com/dslisleedh/dslisleedh_cv/blob/main/ais_ad_aad_model.png)  
      We've considered 2 ways to detect anomalies in maritime AIS data: time-series based anomaly detection and image-based anomaly detection.
I tested image-based anomaly detection, which converts AIS data into track images and uses them as a feature for computational efficiency. It was hard to use existing research because our ROI covered the whole Daehan Strait and Mokpo Sea, but their ROI was only within a specific port. So I proposed a new model architecture which can recognize both track's shape and position in ROI and It showed better performance than time-series based model in our test dataset.

## Education  
 - <b>Kangnam Univ.</b> (Mar. 2016 ~ Feb. 2022)  
   - Department of Library Information Science  
   - Thesis: Analysis of book characteristics that affect book lending 
   - GPA: 3.58 / 4.5  

## Research Interests  
 - Computer Vision
   - Low-level vision task  
 - Generative Models  
 - Low-complexity models
 
 <details>
 <summary> <b>Model Implementations(Click!)</b> </summary>
 
 ### Computer Vision Models  
  - DualPatchNorm [[Tensorflow2/Keras]](https://github.com/dslisleedh/DualPatchNorm-tensorflow2)
  - ConvNeXt [[Tensorflow2/Keras]](https://github.com/dslisleedh/ConvNeXt-tensorflow2)
  - EnsNet [[Tensorflow2/Keras]](https://github.com/dslisleedh/EnsNet-tensorflow2)
  - MetaFormer(PoolFormer) [[Flax]](https://github.com/dslisleedh/MetaFormer-flax)
  - VisionPermutator [[Flax]](https://github.com/dslisleedh/MLP_based_models-flax/blob/main/vip.py)
  - MLPMixer [[Tensorflow2/Keras]](https://github.com/dslisleedh/MLP_based_models-tensorflow2/blob/master/mlpmixer.py) [[Flax]](https://github.com/dslisleedh/MLP_based_models-flax/blob/main/mlpmixer.py)
  - S^2MLP [[Tensorflow2/Keras]](https://github.com/dslisleedh/MLP_based_models-tensorflow2/blob/master/s2mlp.py) [[Flax]](https://github.com/dslisleedh/MLP_based_models-flax/blob/main/s2mlp.py)
  - S^2MLP v2 [[Flax]](https://github.com/dslisleedh/MLP_based_models-flax/blob/main/s2mlpv2.py)
  - gMLPs [[Tensorflow2/Keras]](https://github.com/dslisleedh/MLP_based_models-tensorflow2/blob/master/gmlp.py)
  - ResMLP [[Tensorflow2/Keras]](https://github.com/dslisleedh/MLP_based_models-tensorflow2/blob/master/resmlp.py)  
  - RaftMLP [[Tensorflow2/Keras]](https://github.com/dslisleedh/MLP_based_models-tensorflow2/blob/master/raftmlp.py)  
  - FNet [[Tensorflow2/Keras]](https://github.com/dslisleedh/MLP_based_models-tensorflow2/blob/master/fnet.py)  
  - GFNet [[Tensorflow2/Keras]](https://github.com/dslisleedh/MLP_based_models-tensorflow2/blob/master/gfnet.py)  
  - ConvMLP [[Tensorflow2/Keras]](https://github.com/dslisleedh/MLP_based_models-tensorflow2/blob/master/convmlp.py)  
  - Vision Transformer [[Tensorflow2/Keras]](https://github.com/dslisleedh/VisionTransformers-tensorflow2)   
  - MobileNetV1 [[Flax]](https://github.com/dslisleedh/CNNs-flax/blob/c83548d65e94dffb0fb382bc60854b76178c06c0/src/models.py#L235)  
  - SENet [[Tensorflow2/Keras]](https://github.com/dslisleedh/CNNs-tensorflow2/tree/main/6SENet) [[Flax]](https://github.com/dslisleedh/CNNs-flax/blob/c83548d65e94dffb0fb382bc60854b76178c06c0/src/models.py#L203)
  - DenseNet [[Tensorflow2/Keras]](https://github.com/dslisleedh/CNNs-tensorflow2/tree/main/5DenseNet) [[Flax]](https://github.com/dslisleedh/CNNs-flax/blob/c83548d65e94dffb0fb382bc60854b76178c06c0/src/models.py#L171)
  - PreActResNet [[Flax]](https://github.com/dslisleedh/CNNs-flax/blob/c83548d65e94dffb0fb382bc60854b76178c06c0/src/models.py#L134)
  - ResNet [[Tensorflow2/Keras]](https://github.com/dslisleedh/CNNs-tensorflow2/tree/main/4ResNet) [[Flax]](https://github.com/dslisleedh/CNNs-flax/blob/c83548d65e94dffb0fb382bc60854b76178c06c0/src/models.py#L101)
  - Inception [[Tensorflow2/Keras]](https://github.com/dslisleedh/CNNs-tensorflow2/tree/main/3Inception) [[Flax]](https://github.com/dslisleedh/CNNs-flax/blob/c83548d65e94dffb0fb382bc60854b76178c06c0/src/models.py#L14)
  - VGGNet [[Tensorflow2/Keras]](https://github.com/dslisleedh/CNNs-tensorflow2/tree/main/2VGGNet) [[Flax]](https://github.com/dslisleedh/CNNs-flax/blob/c83548d65e94dffb0fb382bc60854b76178c06c0/src/models.py#L72)
  - AlexNet [[Tensorflow2/Keras]](https://github.com/dslisleedh/CNNs-tensorflow2/tree/main/1AlexNet) 

#### Low level vision task
  - NAFNet [[Tensorflow2/Keras]](https://github.com/dslisleedh/NAFNet-tensorflow2) [[Flax]](https://github.com/dslisleedh/NAFNet-flax/blob/main/nafnet.py)
  - NAFSSR [[Flax]](https://github.com/dslisleedh/NAFNet-flax/blob/main/nafssr.py)
  - NCNet [[Flax]](https://github.com/dslisleedh/NCNet-flax)
  - TR-MISR [[Tensorflow2/Keras]](https://github.com/dslisleedh/TR_MISR)
  - RAMs [[Tensorflow2/Keras]](https://github.com/dslisleedh/SuperResolution-tensorflow2/blob/main/multiimage/rams.py)
  - SwinIR [[Tensorflow2/Keras]](https://github.com/dslisleedh/SwinIR-tensorflow)
  - BTSRN [[Tensorflow2/Keras]](https://github.com/dslisleedh/SuperResolution-tensorflow2/blob/main/singleimage/btsrn.py)
  - CARN [[Tensorflow2/Keras]](https://github.com/dslisleedh/SuperResolution-tensorflow2/blob/main/singleimage/carn.py)
  - DRRN [[Tensorflow2/Keras]](https://github.com/dslisleedh/SuperResolution-tensorflow2/blob/main/singleimage/drrn.py)
  - EDSR [[Tensorflow2/Keras]](https://github.com/dslisleedh/SuperResolution-tensorflow2/blob/main/singleimage/edsr.py)
  - ESPCN [[Tensorflow2/Keras]](https://github.com/dslisleedh/SuperResolution-tensorflow2/blob/main/singleimage/espcn.py)
  - FSRCNN [[Tensorflow2/Keras]](https://github.com/dslisleedh/SuperResolution-tensorflow2/blob/main/singleimage/fsrcnn.py)
  - IRCNN [[Tensorflow2/Keras]](https://github.com/dslisleedh/SuperResolution-tensorflow2/blob/main/singleimage/ircnn.py)
  - MAMNet [[Tensorflow2/Keras]](https://github.com/dslisleedh/SuperResolution-tensorflow2/blob/main/singleimage/mamnet.py)
  - REDNet [[Tensorflow2/Keras]](https://github.com/dslisleedh/SuperResolution-tensorflow2/blob/main/singleimage/rednet.py)
  - SRCNN [[Tensorflow2/Keras]](https://github.com/dslisleedh/SuperResolution-tensorflow2/blob/main/singleimage/srcnn.py)
  - SRGAN [[Tensorflow2/Keras]](https://github.com/dslisleedh/SuperResolution-tensorflow2/blob/main/singleimage/srgan.py)
  - SRRAM [[Tensorflow2/Keras]](https://github.com/dslisleedh/SuperResolution-tensorflow2/blob/main/singleimage/srram.py)
  - VDSR [[Tensorflow2/Keras]](https://github.com/dslisleedh/SuperResolution-tensorflow2/blob/main/singleimage/vdsr.py)
  
### Generative Models  
  - VAE [[Tensorflow2/Keras]](https://github.com/dslisleedh/GenerativeAutoencoders-tensorflow2/blob/main/vae.py) [[Flax]](https://github.com/dslisleedh/Generative_models-flax/blob/1b4bce4529b7098c10493ee2673bb2df59ddde2f/src/models.py#L21)
  - MarkovianHVAE [[Flax]](https://github.com/dslisleedh/Generative_models-flax/blob/1b4bce4529b7098c10493ee2673bb2df59ddde2f/src/models.py#L48)
  - AAE [[Tensorflow2/Keras]](https://github.com/dslisleedh/GenerativeAutoencoders-tensorflow2/blob/main/aae.py)
  - CAAE [[Tensorflow2/Keras]](https://github.com/dslisleedh/GenerativeAutoencoders-tensorflow2/blob/main/caae.py)
  - DFCVAE [[Tensorflow2/Keras]](https://github.com/dslisleedh/GenerativeAutoencoders-tensorflow2/blob/main/dfcvae.py)
  - GAN [[Tensorflow2/Keras]](https://github.com/dslisleedh/GAN-tensorflow2/blob/master/gan.py) [[Flax]](https://github.com/dslisleedh/Generative_models-flax/blob/1b4bce4529b7098c10493ee2673bb2df59ddde2f/src/models.py#L102)
  - CGAN [[Tensorflow2/Keras]](https://github.com/dslisleedh/GAN-tensorflow2/blob/master/cgan.py)
  - DCGAN [[Tensorflow2/Keras]](https://github.com/dslisleedh/GAN-tensorflow2/blob/master/dcgan.py)
  - LSGAN [[Tensorflow2/Keras]](https://github.com/dslisleedh/GAN-tensorflow2/blob/master/lsgan.py)
  - WGAN [[Tensorflow2/Keras]](https://github.com/dslisleedh/GAN-tensorflow2/blob/master/wgan.py)
  - WGAN-gp [[Tensorflow2/Keras]](https://github.com/dslisleedh/GAN-tensorflow2/blob/master/wgangp.py)
  - CycleGAN [[Tensorflow2/Keras]](https://github.com/dslisleedh/GAN-tensorflow2/blob/master/cyclegan.py)
 </details>
   
   
## Things I can do ...
  - Implement models in various frameworks(TF2/Keras, Pytorch, Flax(<b>Contributor</b>)). 
  - Propose a new model architecture suitable for the situation.
  
 
