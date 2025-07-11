# Darknet-Y7-ConvCBAM-SwinT
A repo that demonstrates the integration of my custom ConvCBAM and SwinTransformer-based attention mechanisms to enhance the performance of the YOLOv7 architecture.
This is an ongoing project where I am actively overhauling and pushing the capabilities of YOLOv7.

# Performance Increases:

ConvCBAM-enhanced YOLOv7 trained from scratch on the INsPLAD dataset achieves:

+11.2% improvement in mAP@0.5

+4.6% improvement in mAP@0.5:0.95
compared to a pretrained baseline YOLOv7.

Faster convergence:

Strategically placed ConvCBAM modules reduce the number of images and epochs needed to reach comparable performance by approximately 22% and 35% respectively, demonstrated on:

the Smoke-Fire Detection YOLO dataset on Kaggle

and an in-house dataset.

CBAMSlidingWindowBlock-equipped YOLOv7 shows:

+3.2% increase in precision (P)

+2.7% increase in recall (R)
over the base YOLOv7-large on the COCO dataset after just 10 epochs.

# Why this matters:

Both of my enhanced architectures — particularly ConvCBAM — directly address common weaknesses in YOLOv7 and other object detectors by significantly improving the model's ability to:

Detect small objects

Recognize objects in busy scenes

Handle densely packed instances

The combination of channel and spatial attention dramatically refines the way the network learns feature representations.
Additionally, the Sliding Window + CBAM approach greatly boosts the model's ability to not only focus on the most important features but also capture contextual relationships within local windows.

# TLDR:
My work systematically upgrades YOLOv7 to be more context-aware, more efficient, and substantially more powerful for challenging detection tasks.

