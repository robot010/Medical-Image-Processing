# Medical-Image-Processing
This repository contains some works that I have done in [Computation Radiology Lab UR Medical Center](https://www.urmc.rochester.edu/labs/wismueller.aspx).

It mainly contains the following parts:

- Phase contrast X-ray computed tomography (PCI-CT) deep learning classifier. 
- Vertebrae Segmentation in Pathological Spine CT via Fully Convolutional Neural Network.
- Preprocessing of Raw image data (.mhd/.raw/.dicom) of [Annotated lymph node CT dataset](http://www.holgerroth.com/data) and [Microsoft's Spine Web dataset](https://www.dropbox.com/sh/kbnzg63447hx3eq/AACy8dQ01YM-0IEwYK4vVJ3Na?dl=0)


## Keypoints of PCT-CT deep learning project

- This project got accepted at SPIE2017 conference for oral representation. You can check out our publication [here](http://spie.org/Publications/Proceedings/Paper/10.1117/12.2254645). A refined version of this paper is uploaded [here](https://github.com/Bato803/Medical-Image-Processing/blob/master/Deep_Transfer_Learning_PCI_CT.pdf). 

- It makes fully use of CaffeNet and Inception-v3 Net to classify CT samples. Please check out `Deep_Transfer_Learning_PCI_CT.pdf` for full detail. 

- Some result is shown below:
  
  The classification result we got from a fine-tuned CaffeNet. 
  <img src="https://user-images.githubusercontent.com/17235054/31979049-a629dc94-b912-11e7-8d84-2d52c3180533.png" width=800 height=300>
  
  
  ## Keypoints of Vertebrea Segmentation project
  
- Preprocessing raw spine dataset (About 20GB), you can check out the sample spine CT scan before and after preprocessing below. 

The preprocessing techniques we have explored include: [Histogram Equalization](https://en.wikipedia.org/wiki/Histogram_equalization), [Adaptive Histogram Equalization](https://en.wikipedia.org/wiki/Adaptive_histogram_equalization) and [Constrast Stretching](http://what-when-how.com/embedded-image-processing-on-the-tms320c6000-dsp/contrast-stretching-image-processing/)

  <img src="https://user-images.githubusercontent.com/17235054/31979465-dc29dfc2-b914-11e7-8d3f-3abe507bb7ca.png" width=300
  height=100>
  
  <img src="https://user-images.githubusercontent.com/17235054/31979468-e33bf160-b914-11e7-924d-e4544f300839.png" width=200 height=300>
  
  For full detail, please refers to our report [here](https://github.com/Bato803/Medical-Image-Processing/blob/master/egpaper_final.pdf). 
    

 
 - Prepared the lmdb file so that the data can be directly fed into Convolutional Neural Network. 
 
 - Used fully convolutional neural network to segment the image. 
  
