<p align="center"><img src="awesome-tflite.png" /></p>

# Awesome TFLite [![Awesome](https://awesome.re/badge.svg)](https://awesome.re) [![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg?style=flat-square)](http://makeapullrequest.com) ![Twitter Follow](https://img.shields.io/twitter/follow/margaretmz?label=%40margaretmz&style=social)
TensorFlow Lite (TFLite) is a set of tools that help convert TensorFlow models to run on mobile and edge devices - currently running on more than 3 billion devices! 

This is a curated list of TFLite models with sample apps, model zoo, helpful tools and learning resources. Please submit a PR if you would like to contribute and follow the guidelines [here](CONTRIBUTING.md).

## New features
Here are some new features recently announced at TensorFlow World:
* TFLite Android Support Library - [documentation](https://github.com/tensorflow/tensorflow/tree/master/tensorflow/lite/experimental/support/java) | Sample code ([Android](https://github.com/tensorflow/examples/blob/master/lite/examples/image_classification/android/EXPLORE_THE_CODE.md))
* Transfer learning made easy with model customization API -  Colab tutorials - [Image](https://github.com/tensorflow/examples/blob/master/tensorflow_examples/lite/model_customization/demo/image_classification.ipynb) | [Text](https://github.com/tensorflow/examples/blob/master/tensorflow_examples/lite/model_customization/demo/text_classification.ipynb)
* On-device training is finally here - [Blog](https://blog.tensorflow.org/2019/12/example-on-device-model-personalization.html) | Sample code ([Android](https://github.com/tensorflow/examples/blob/master/lite/examples/model_personalization/README.md))
* Accelerating TensorFlow Lite on Qualcomm Hexagon DSPs - [Blog](https://blog.tensorflow.org/2019/12/accelerating-tensorflow-lite-on-qualcomm.html) | [Documentation](https://github.com/tensorflow/tensorflow/blob/master/tensorflow/lite/g3doc/performance/hexagon_delegate.md)

## TFLite models
Here are the TFLite models with app / device implementations, and references.
Note: pretrained TFLite models from MediaPipe are included, which you can implement with or without MediaPipe. 

### Computer vision

| Task           | Model         | App \| Reference                        | Source |
| -------------- |---------------| -------------------------------------- | --------- |
| Classification | MobileNetV1 ([download](https://storage.googleapis.com/download.tensorflow.org/models/tflite/mobilenet_v1_1.0_224_quant_and_labels.zip))| [Android](https://github.com/tensorflow/examples/tree/master/lite/examples/image_classification/android) \| [iOS](https://github.com/tensorflow/examples/tree/master/lite/examples/image_classification/ios) \| [Raspberry Pi](https://github.com/tensorflow/examples/tree/master/lite/examples/image_classification/raspberry_pi) \| [Overview](https://www.tensorflow.org/lite/models/image_classification/overview)| tensorflow.org |
| Classification | MobileNetV2   | Skin Lesion Detection [Android](https://github.com/AakashKumarNain/skin_cancer_detection/tree/master/demo)|Community|
| Object detection | Quantized COCO SSD MobileNet v1 ([download](https://storage.googleapis.com/download.tensorflow.org/models/tflite/coco_ssd_mobilenet_v1_1.0_quant_2018_06_29.zip)) | [Android](https://github.com/tensorflow/examples/tree/master/lite/examples/object_detection/android) \| [iOS](https://github.com/tensorflow/examples/tree/master/lite/examples/object_detection/ios) \| [Overview](https://www.tensorflow.org/lite/models/object_detection/overview#starter_model) | tensorflow.org |
| Object detection | YOLO        | [Flutter](https://blog.francium.tech/real-time-object-detection-on-mobile-with-flutter-tensorflow-lite-and-yolo-android-part-a0042c9b62c6) \| [Paper](https://arxiv.org/abs/1506.02640)  | Community |
| Object detection | MobileNetV2 SSD ([download](https://github.com/google/mediapipe/tree/master/mediapipe/models/ssdlite_object_detection.tflite)) | [Reference](https://github.com/google/mediapipe/blob/master/mediapipe/models/object_detection_saved_model/README.md) | MediaPipe |
| License Plate detection | SSD MobileNet [(download)](https://github.com/ariG23498/Flutter-License/blob/master/assets/detect.tflite) | [Flutter](https://github.com/ariG23498/Flutter-License) | Community |
| Face detection | BlazeFace ([download](https://github.com/google/mediapipe/tree/master/mediapipe/models/face_detection_front.tflite)) | [Paper](https://sites.google.com/corp/view/perception-cv4arvr/blazeface) \| [Model card](https://sites.google.com/corp/view/perception-cv4arvr/blazeface#h.p_21ojPZDx3cqq) | MediaPipe |
|Hand detection & tracking | Download: <br> [Palm detection](https://github.com/google/mediapipe/tree/master/mediapipe/models/palm_detection.tflite), <br> [2D hand landmark](https://github.com/google/mediapipe/tree/master/mediapipe/models/hand_landmark.tflite), <br> [3D hand landmark](https://github.com/google/mediapipe/tree/master/mediapipe/models/hand_landmark_3d.tflite) | [Blog post](https://mediapipe.page.link/handgoogleaiblog) \| [Model card](https://mediapipe.page.link/handmc) | MediaPipe |
| Pose estimation | Posenet ([download](https://storage.googleapis.com/download.tensorflow.org/models/tflite/posenet_mobilenet_v1_100_257x257_multi_kpt_stripped.tflite)) | [Android](https://github.com/tensorflow/examples/tree/master/lite/examples/posenet/android) \| [Overview](https://www.tensorflow.org/lite/models/pose_estimation/overview)| tensorflow.org |
| Segmentation | DeepLab V3 ([download](https://storage.googleapis.com/download.tensorflow.org/models/tflite/gpu/deeplabv3_257_mv_gpu.tflite)) |  [Flutter](https://github.com/kshitizrimal/Flutter-TFLite-Image-Segmentation) \| [Paper](https://arxiv.org/abs/1706.05587) | Community |
Segmentation (Flutter Realtime) | DeepLab V3 ([download](https://storage.googleapis.com/download.tensorflow.org/models/tflite/gpu/deeplabv3_257_mv_gpu.tflite)) |  [Flutter](https://github.com/kshitizrimal/tflite-realtime-flutter) \| [Paper](https://arxiv.org/abs/1706.05587) | Community |
| Segmentation | DeepLab V3 ([download](https://storage.googleapis.com/download.tensorflow.org/models/tflite/gpu/deeplabv3_257_mv_gpu.tflite)) | [Android](https://github.com/tensorflow/examples/tree/master/lite/examples/image_segmentation/android) \| [iOS](https://github.com/tensorflow/examples/tree/master/lite/examples/image_segmentation/ios) \| [Overview](https://www.tensorflow.org/lite/models/style_transfer/overview)  | tensorflow.org |
| Hair Segmentation | [Download](https://github.com/google/mediapipe/tree/master/mediapipe/models/hair_segmentation.tflite) | [Paper](https://sites.google.com/corp/view/perception-cv4arvr/hair-segmentation) \| [Model card](https://sites.google.com/corp/view/perception-cv4arvr/hair-segmentation#h.p_NimuO7PgHxlY) | MediaPipe |
| Style transfer |  Download: <br> [Style prediction](https://storage.googleapis.com/download.tensorflow.org/models/tflite/arbitrary_style_transfer/style_predict_quantized_256.tflite), <br> [Style transform](https://storage.googleapis.com/download.tensorflow.org/models/tflite/arbitrary_style_transfer/style_transfer_quantized_dynamic.tflite) | [Overview](https://www.tensorflow.org/lite/models/style_transfer/overview) | tensorflow.org|

### Text
| Task           | Model         | App \| Reference                       | Source    |
| -------------- |---------------| -------------------------------------- | --------- |
| Question & Answer | DistilBERT | [Android](https://github.com/huggingface/tflite-android-transformers/blob/master/bert) | Hugging Face |
| Text Generation | GPT-2 / DistilGPT2 | [Android](https://github.com/huggingface/tflite-android-transformers/blob/master/gpt2) | Hugging Face |
### Speech
| Task               | Model    | App \| Reference    | Source    |
| ------------------ |----------| ------------------- | --------- |
| Speech Recognition | DeepSpeech | [Reference](https://github.com/mozilla/DeepSpeech/tree/master/native_client/java) | Mozilla |

## TFLite model zoo
TFLite models that could be implemented in apps and things:
*  [MobileNet](https://github.com/tensorflow/models/blob/master/research/slim/nets/mobilenet/README.md)- pretrained MobileNet v2 and v3 models.
* TFLite models
    * [TensorFlow Lite models](https://www.tensorflow.org/lite/models) with Android and iOS examples
    * [TensorFlow Lite hosted models](https://www.tensorflow.org/lite/guide/hosted_models) with quantized and floating point variants 
    * [TFLite models from TensorFlow Hub](https://tfhub.dev/s?q=tflite)

## TensorFlow model zoo
TensorFlow models that could be converted to TFLite and then implemented in apps and things:
* [Official TensorFlow models](https://github.com/tensorflow/models/tree/master/official)
* [Tensorflow detection model zoo](https://github.com/tensorflow/models/blob/master/research/object_detection/g3doc/detection_model_zoo.md) -
pre-trained on COCO, KITTI,  AVA v2.1, iNaturalist Species datasets)

## ML Kit examples
* 2/9/219 Flutter + MLKit: Business Card Mail Extractor - [tutorial](https://medium.com/flutter-community/flutter-mlkit-8039ec66b6a) | [Flutter](https://github.com/DaemonLoki/Business-Card-Mail-Extractor) 
* 2/8/2019 From TensorFlow to ML Kit: Power your Android application with machine learning - [slides](https://speakerdeck.com/jinqian/from-tensorflow-to-ml-kit-power-your-android-application-with-machine-learning) | [Android](https://github.com/xebia-france/magritte) (Kotlin)
* 8/7/2018 Building a Custom Machine Learning Model on Android with TensorFlow Lite - [tutorial](https://medium.com/over-engineering/building-a-custom-machine-learning-model-on-android-with-tensorflow-lite-26447e53abf2)
* 7/27/2018 ML Kit on Android 4: Landmark Detection - [tutorial](https://medium.com/google-developer-experts/exploring-firebase-mlkit-on-android-landmark-detection-part-four-5e86b8deac3a)
* 7/28/2018 ML Kit on Android 3: Barcode Scanning - [tutorial](https://medium.com/google-developer-experts/exploring-firebase-mlkit-on-android-barcode-scanning-part-three-cc6f5921a108)
* 5/31/2018 ML Kit on Android 2: Face Detection - [tutorial](https://medium.com/google-developer-experts/exploring-firebase-mlkit-on-android-face-detection-part-two-de7e307c52e0)
* 5/22/2018 ML Kit on Android 1: Intro - [tutorial](https://medium.com/google-developer-experts/exploring-firebase-mlkit-on-android-introducing-mlkit-part-one-98fcfedbeee0)

## Other
* [Coral Edge TPU examples](https://coral.ai/examples/)
* [MediaPipe examples](https://mediapipe.readthedocs.io/en/latest/examples.html): mobile, desktop and Edge TPUs
* [TensorFlow Lite for Microcontrollers](https://www.tensorflow.org/lite/microcontrollers)

## Helpful links
* [Netron](https://github.com/lutzroeder/netron) - for visualizing models
* [AI benchmark](http://ai-benchmark.com/tests.html)  - for benchmarking computer vision models on smartphones
* [Performance benchmarks](https://www.tensorflow.org/lite/performance/benchmarks) for Android and iOS
* How to design machine learning powered features - [material design guidelines for ML](https://material.io/collections/machine-learning/patterns-for-machine-learning-powered-features.html) | [ML Kit Showcase App](https://github.com/firebase/mlkit-material-android)
* [The People + AI Guide book](https://pair.withgoogle.com/) - learn how to design human-centered AI products

## Learning resources
Interested but not sure how to get started? Here are some learning resources that will help you whether you are a beginner or a practitioner in the field for a while.

### Documentation
* Official TensorFlow Lite documentation ([link](https://www.tensorflow.org/lite))

### Blog posts 
* 11/8/2019 - Getting  Started with ML on MCUs with TensorFlow ([link](https://blog.particle.io/2019/11/08/particle-machine-learning-101/))
* 8/5/2019 - TensorFlow Model Optimization Toolkit — float16 quantization halves model size  ([link](https://blog.tensorflow.org/2019/08/tensorflow-model-optimization-toolkit_5.html))
* 7/13/2018 - Training and serving a realtime mobile object detector in 30 minutes with Cloud TPUs  ([link](https://blog.tensorflow.org/2018/07/training-and-serving-realtime-mobile-object-detector-cloud-tpus.html))
* 6/11/2018 - Why the Future of Machine Learning is Tiny  ([link](https://petewarden.com/2018/06/11/why-the-future-of-machine-learning-is-tiny/))
* 3/30/2018 - Using TensorFlow Lite on Android ([link](https://blog.tensorflow.org/2018/03/using-tensorflow-lite-on-android.html))

### Books
* 12/2019 - [TinyML](http://shop.oreilly.com/product/0636920254508.do)  by Pete Warden ([@petewarden](https://twitter.com/petewarden)), Daniel Situnayake ([@dansitu](https://twitter.com/dansitu)) 
* 10/2019 - [Practical Deep Learning for Cloud, Mobile, and Edge](https://www.practicaldeeplearning.ai/) by Anirudh Koul ([@AnirudhKoul](https://twitter.com/AnirudhKoul)), Siddha Ganju ([@SiddhaGanju](https://twitter.com/SiddhaGanju)), and Meher Kasam ([@MeherKasam](https://twitter.com/MeherKasam))

### YouTube videos
* 10/31/2019 - [Keynote - TensorFlow Lite: ML for mobile and IoT devices](https://www.youtube.com/watch?v=zjDGAiLqGk8) 
* 10/31/2019 - [TensorFlow Lite: Solution for running ML on-device](https://www.youtube.com/watch?v=0SpZy7iouFU)
* 10/31/2019 - [TensorFlow model optimization: Quantization and pruning](https://www.youtube.com/watch?v=3JWRVx1OKQQ) 
* 10/29/2019 - [Inside TensorFlow: TensorFlow Lite](https://www.youtube.com/watch?v=gHN0jDbJz8E&t=540s)
* 4/18/2018 - [TensorFlow Lite for Android (Coding TensorFlow)](https://www.youtube.com/watch?v=JnhW5tQ_7Vo&t=22s)

### MOOC
* Udacity [Introduction to TensorFlow Lite](https://www.udacity.com/course/intro-to-tensorflow-lite--ud190) - by Daniel Situnayake ([@dansitu](https://twitter.com/dansitu)), Paige Bailey ([@DynamicWebPaige](https://twitter.com/DynamicWebPaige)), and Juan Delgado
* Coursera [Device-based Models with TensorFlow Lite](https://www.coursera.org/learn/device-based-models-tensorflow) - by Laurence Moroney ([@lmoroney](https://twitter.com/lmoroney))




