# Medical-Image-segmentation
Medical Image Segmentation plays a key role in diagnosis and treatment. The deep neural network called
DeepLabV3 is used to detect the polyps in colonoscopy images.The model is examined with the
CVC-ClinicDB dataset, is a database of frames extracted from colonoscopy videos. After
training with 267 images and testing with 345 images, we got a good performance, 98.2% mean
Intersection over Union (mIOU). Once the trained model is applied to clinical colonoscopy exam
videos, it could provide effective opinions in real time to aid the diagnosis.

**What is Semantic Segmentation?**
The goal of semantic image segmentation is to label each pixel of an image with a
corresponding class of what is being represented. If you have two objects of the same category in
your input image, the segmentation map does not inherently distinguish these as separate objects.

**How to implement Segmentation?**
”segmentation_models_pytorch” library is used for segmentation.
The main features of this library are:
 High level API (just two lines to create neural network)
 5 models architectures for binary and multi class segmentation (including legendary
Unet)
 46 available encoders for each architecture
 All encoders have pre-trained weights for faster and better convergence

**Why Do We Need Image Augmentation?**
Deep learning models usually require a lot of data for training. In general, the more the data, the
better the performance of the model. But acquiring massive amounts of data comes with its own
challenges. Not everyone has the deep pockets of the big firms and the problem with a lack of
data is that our deep learning model might not learn the pattern or function from the data and
hence it might not give a good performance on unseen data.So, we can make use of Image
Augmentation techniques.

**DeepLabV3+**
DeepLab_v3+ has the highest performance about mean Intersection over Union (mIoU)
for object detection.It consists of three sub-frameworks, ResNet, multi-grid methods, and ASPP
in cascade. ResNet-50 performs better than ResNet-101 because the latter one compresses more
information about the image, which results in losing polyps signal. The multi-grid methods and
ASPP approach result in a wider field-ofview and higher resolution in the processed feature
responses.

**ResNet-50**
ResNet-50 is a convolutional neural network that is 50 layers deep. You can load a
pretrained version of the network trained on more than a million images from the ImageNet
database. The pretrained network can classify images into 1000 object categories. A
network has learned rich feature representations for a wide range of images.
