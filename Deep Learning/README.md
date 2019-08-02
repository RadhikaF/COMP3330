# Deep Learning Project
The aim of this project was to use deep neural networks to develop a basic computer vision system for autonomous drones that can detect and localise plastic bottles and cans in video frames so that they can be collected. 

The task rquired the development and annotation of a dataset which we acquired by taking images of bottles and cans in a variety of outdoor locations using a mobile phone camera. To add to the bulk of the dataset, models of cans and bottles were synthetically generated using Blender 2.79b and placed randomly within 360 degree High Dynamic Range (HDR) images. The bounding boxes were drawn around the cans and bottles using the image annotation tool, LabelImg (https://github.com/tzutalin/labelImg). 

I implemented transfer learning with the Single Shot MultiBox Detector model, specifically using the SSD300 network architecture. Our training was based upon the SSD300 Keras implementation at https://github.com/pierluigiferrari/ssd_keras. This network has been trained on the PascalVOC 2007 dataset which contains 20 object classes. To train the original SSD300 model on our own dataset, we sub-sampled the weight tensors of the classification layers for fully convolutionalised SSD300 model.

The results of the model are contained in the report.
