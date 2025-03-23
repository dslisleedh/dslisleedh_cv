<h1>
<div align="center">
  이동헌(Dongheon Lee, dslisleedh)
</div>
</h1>

<div align="right">
  <b>Birth:</b> 12/22/1997

  <b>Email:</b> dslisleedh@gmail.com, dslisleedh@uos.ac.kr
</div>

## Career  
 - UST21 (Research & Development department)
   - AI Engineer (Mar. 2022 ~ Apr. 2023)  
   - Work experiences  
     - <b>Sea-Surface-Temperature super resolution</b> (July 2022 ~ Apr. 2023)  
       ![SST_SR_result](https://github.com/dslisleedh/dslisleedh_cv/blob/main/sst_sr_result.PNG)
       To enhance the resolution of sea surface temperature (SST) data from remote sensing, I evaluated two approaches: Single Image Super-Resolution (SISR) and Multi-Image Super-Resolution (MISR). I selected NAFSR (Non-linear Activate Free Network for Super-Resolution) for SISR due to its simplicity, and TR-MISR for MISR as it is the state-of-the-art model on the unique PROBA-V MISR dataset. The SISR approach (NAFSR) achieved superior performance, with a PSNR improvement of +0.97 dB over MISR and +1.34 dB over bicubic interpolation at a scale factor of 4.
       
     - <b>Sea-fog generation prediction</b> (Apr. 2022 ~ Dec. 2022)  
        I evaluated various models to address a highly imbalanced time-series classification task. After completing training, I deployed the model into production. The models tested included:
          - Transformer
          - GFNet
          - Large Kernel Convolution based model

     - <b>Anomaly detection on maritime AIS data</b> (May 2022 ~ Nov. 2022)  
       ![Model](https://github.com/dslisleedh/dslisleedh_cv/blob/main/ais_ad_aad_model.png)  
      We explored two approaches for detecting anomalies in maritime AIS data: time-series-based anomaly detection and image-based anomaly detection. I focused on the image-based approach, which converts AIS data into track images to serve as computationally efficient features. Since our region of interest (ROI) spanned the entire Daehan Strait and Mokpo Sea—unlike previous studies that concentrated on specific port areas—I proposed a novel model architecture that recognizes both the shape and location of tracks within the ROI. This approach outperformed the time-series-based model on our test dataset.


## Papers
 - Arbitrary-Scale Downscaling of Tidal Current Data Using Implicit Continuous Representation ([[IEEE Access]](https://arxiv.org/abs/2401.15893), 2024)
 - PLKSR: Partial Large Kernel CNNs for Efficient Super-Resolution ([[Arxiv]](https://arxiv.org/pdf/2404.11848.pdf), 2024)
 - IGConv: Implicit Grid Convolution for Multi-Scale Image Super-Resolution ([[Arxiv]](https://arxiv.org/pdf/2408.09674v1), 2024)
 - ESC: Emulating Self-attention with Convolution for Efficient Image Super-Resolution ([[Arxiv]](https://arxiv.org/abs/2503.06671), 2024)
   
## Education  
 - <b>Kangnam Univ.</b> (Mar. 2016 ~ Feb. 2022)  
   - B.S. degree
   - Department of Library Information Science  
   - Thesis: Analysis of book characteristics that affect book lending 
 - <b>University of Seoul</b> (Sep. 2023 ~ Now)
   - M.S. student
   - Department of Artificial Intelligence

## Research Interests  
 - Computer Vision
 - Image Processing
   - Super-Resolution (Image, Burst Image, and Video)
 - Computational Efficiency
   
## Things I can do ...
  - Implement models in various frameworks(TF2/Keras, Pytorch, Flax(<b>Contributor</b>)). 
  - Propose innovative model architectures tailored to specific needs.
  
 
