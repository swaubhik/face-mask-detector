<h1 align="center">Face Mask Detector</h1>

<div align= "center">
  <h4>Face Mask Detection system built with OpenCV, Keras/TensorFlow using Deep Learning and Computer Vision concepts in order to detect face masks in static images as well as in real-time video streams.</h4>
</div>
<p align="center">
![Live Demo](https://github.com/swaubhik/face-mask-detector/blob/master/Readme_images/demo.gif)
</p>
## :innocent: Motivation

In the present scenario due to Covid-19, there is no efficient face mask detection applications which are now in high demand for transportation means, densely populated areas, residential districts, large-scale manufacturers and other enterprises to ensure safety. Also, the absence of large datasets of **‘with_mask’** images has made this task more cumbersome and challenging.

## :eyes: Demo image

<p align="center"><img src="https://github.com/swaubhik/face-mask-detector/blob/master/Readme_images/demo.jpg" width="700" height="400"></p>
<p align="center"><img src="<p align="center"><img src="https://github.com/swaubhik/face-mask-detector/blob/master/Readme_images/demo_nomask1.jpg" width="700" height="400"></p>

## :warning: TechStack/framework used

- [OpenCV](https://opencv.org/)
- [Caffe-based face detector](https://caffe.berkeleyvision.org/)
- [Keras](https://keras.io/)
- [TensorFlow](https://www.tensorflow.org/)
- [MobileNetV2](https://arxiv.org/abs/1801.04381)

## :star: Features

Our face mask detector didn't use any morphed masked images dataset. The model is accurate, and since we used the MobileNetV2 architecture, it’s also computationally efficient and thus making it easier to deploy the model to embedded systems (Raspberry Pi, Google Coral, etc.).

This system can therefore be used in real-time applications which require face-mask detection for safety purposes due to the outbreak of Covid-19. This project can be integrated with embedded systems for application in airports, railway stations, offices, schools, and public places to ensure that public safety guidelines are followed.

## :file_folder: Dataset

The dataset used can be downloaded here - [Click to Download](https://drive.google.com/drive/folders/144CEMv7po2GD1Ea8XPirTZ8-OflINcoC?usp=sharing)

This dataset consists of **4095 images** belonging to two classes:

- **with_mask: 2165 images**
- **without_mask: 1930 images**

The images used were real images of faces wearing masks. The images were collected from the following sources:

- **Bing Search API**
- **Kaggle datasets**
- **RMFD dataset** ([See here](https://github.com/X-zhangyang/Real-World-Masked-Face-Dataset/tree/master/RWMFD_part_1))

## :key: Prerequisites

All the dependencies and required libraries are included in the file <code>requirements.txt</code> [See here](https://github.com/swaubhik/face-mask-detector/blob/master/requirements.txt)

## 🚀&nbsp; Installation

1. Clone the repo

```
$ git clone https://github.com/swaubhik/face-mask-detector.git
```

2. Change your directory to the cloned repo and create a Python virtual environment named 'test'

```
$ mkvirtualenv test
```

3. Now, run the following command in your Terminal/Command Prompt to install the libraries required

```
$ pip install -r requirements.txt
```

## :bulb: Working

1. Open terminal. Go into the cloned project directory and type the following command:

```
$ python train_mask_detector.py --dataset dataset
```

2. To detect face masks in an image type the following command:

```
$ python detect_mask_image.py --image images/pic1.jpeg
```

3. To detect face masks in real-time video streams type the following command:

```
$ python detect_mask_video.py
```

## :key: Results

#### Our model gave 93% accuracy for Face Mask Detection after training via <code>tensorflow-gpu==2.0.0</code>

![](https://github.com/swaubhik/face-mask-detector/blob/master/Readme_images/evaluating.jpg)

#### We got the following accuracy/loss training curve plot

![](https://github.com/swaubhik/face-mask-detector/blob/master/plot.png)

## :clap: And it's done!

Feel free to mail me for any doubts/query
:email: b18csel299@cit.ac.in

## :handshake: Contribution

Feel free to **file a new issue** with a respective title and description on the the [Face-Mask-Detection](https://github.com/swaubhik/face-mask-detector/issues) repository. If you already found a solution to your problem, **I would love to review your pull request**!

## :heart: Owner

Made with :heart:&nbsp; by [Swaubhik Chakraborty](https://github.com/swaubhik)

## :+1: Credits

- [https://www.pyimagesearch.com/](https://www.pyimagesearch.com/)
- [https://www.tensorflow.org/tutorials/images/transfer_learning](https://www.tensorflow.org/tutorials/images/transfer_learning)

## :eyes: License

GNU © [Swaubhik Chakraborty](https://github.com/swaubhik/face-mask-detector/blob/master/LICENSE)
