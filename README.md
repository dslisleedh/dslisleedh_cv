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
       To upscale SST data from remote sensing, I tested two strategies: SISR and MISR. I chose NAFSR (Non-linear Activate Free Network for Super-Resolution) for SISR because of its simplicity, and TR-MISR for MISR because it is the SOTA model in the unique MISR dataset, PROBA-V. SISR (NAFSR) performed best, with a PSNR gain of +0.97 dB over MISR and +1.34 dB over bicubic interpolation at scale 4. 
       
     - <b>Sea-fog generation prediction</b> (Apr. 2022 ~ Dec. 2022)  
        I tested various models to handle an extremely imbalanced time-series classification dataset. After the training is complete, I deploy the model to the actual service.
        Models tested:
          - Transformer
          - GFNet
          - 1D-Convolution based model

     - <b>Anomaly detection on maritime AIS data</b> (May 2022 ~ Nov. 2022)  
       ![Model](https://github.com/dslisleedh/dslisleedh_cv/blob/main/ais_ad_aad_model.png)  
      We've considered 2 ways to detect anomalies in maritime AIS data: time-series based anomaly detection and image-based anomaly detection.
I tested image-based anomaly detection, which converts AIS data into track images and uses them as a feature for computational efficiency. It was hard to use existing research because our ROI covered the whole Daehan Strait and Mokpo Sea, but their ROI was only within a specific port. So I proposed a new model architecture which can recognize both track's shape and position in ROI and It showed better performance than time-series based model in our test dataset.

## Papers
 - Arbitrary-Scale Downscaling of Tidal Current Data Using Implicit Continuous Representation ([[IEEE Access]](https://arxiv.org/abs/2401.15893), 2024)
 - PLKSR: Partial Large Kernel CNNs for Efficient Super-Resolution ([[Arxiv]](https://arxiv.org/pdf/2404.11848.pdf), 2024)
 - IGConv: Implicit Grid Convolution for Multi-Scale Image Super-Resolution ([[Arxiv]](https://arxiv.org/pdf/2408.09674v1), 2024)
   
## Education  
 - <b>Kangnam Univ.</b> (Mar. 2016 ~ Feb. 2022)  
   - B.S. degree
   - Department of Library Information Science  
   - Thesis: Analysis of book characteristics that affect book lending 
 - <b>University of Seoul</b> (Sep. 2023 ~ )
   - M.S. studuent
   - Department of Artificial Intelligence

## Research Interests  
 - Computer Vision
 - Image Processing
   - Super-Resolution   
 - Computational Efficiency
   
## Things I can do ...
  - Implement models in various frameworks(TF2/Keras, Pytorch, Flax(<b>Contributor</b>)). 
  - Propose a new model architecture suitable for the situation.
  
 
