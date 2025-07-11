# Darknet-Y7-ConvCBAM-SwinT
A repo that demonstrates the use of my custom ConvCBAMs and SwinTransformers to ameliorate the performance of the existing Yolov7 architecture. This repo is a WIP where I am trying to overhaul yolov7 

# Performance Increases:

1) My ConvCBAM-equipped Yolov7 trained from-scratch on the INsPLAD dataset boasts a boost of 11.2% in MAP@0.5 scores and 4.6% in MAP@.5-.95 when compared to the scores of a pretrained Yolov7.
2) My strategically placed ConvCBAMs have also reduced the amount of images and epochs needed to train a Yolov7 on a new task and achieve simlar performance by about 22%. Tests were conducted using the: https://www.kaggle.com/datasets/sayedgamal99/smoke-fire-detection-yolo?resource=download dataset and an in-house dataset.
3) My CBAMSlidingWindowBlock equipped Yolov7 boasts an increased P score (by 3.2%) and R score (by 2.7%) when compared to the base yolov7-large on the COCO dataset trained on 10 epochs
4) Both model architectures enhanced by me, (especially ConvCBAM) do a great job at overcoming the weakness of not only yolov7 but also other object detectors by improving the model's ability to aptly capture and detect -
   a) small objects
   b) objects in busy scenes
   c) objects that are tightly packed together
5) The channel and spatial attentions seem to have a great impact on the way the architecture learns
6) Addition of Sliding Window approach on top of CBAM greatly increases the models ability to not only focus on the important features across the channels and across the dimensions, but also the models ability to find the relevance of features with respect to each other inside the windows, leading to the development of context
