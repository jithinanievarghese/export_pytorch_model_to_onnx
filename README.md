# Exporting Pytorch model to onnx format

- This repo is a part for following project 
[Web Scraping with product search relevance using NLP, rules and image classification](https://github.com/jithinanievarghese/product-search-relevance/blob/main/README.md)

- Here we convert a binary [image classifcation](https://github.com/jithinanievarghese/image_classification_pytorch) model trained in pytorch  to [onnx format](https://onnx.ai/)  and then we do inference in [onnxruntime](https://onnxruntime.ai/) without any pytorch dependencies.

## Why do we need ONNX format and ONNXRUNTIME over PyTorch or Tensorflow inference

- The cpu version of deep learning framewok like pytorch alone consumes nearly 700mb of server size
- This can be a bottleneck while deployment, considering the resources and latency in inference.
- [ONNX (Open Neural Network Exchange )](https://onnx.ai/) is an open format built to represent machine learning models  i.e a common file format to enable AI developers to use models with a variety of frameworks, tools, runtimes, and compilers.
- After the coverting the pytorch model to onnx format
- With [onnxruntime](https://onnxruntime.ai/docs/get-started/with-python.html) we can make faster inference without any pytorch or any other deep learning framework dependencies 
- latest [onnxruntime](https://onnxruntime.ai/docs/get-started/with-python.html) total pip package or wheel size is around 15-16mb.
- We can view the model architecture by uploading onnx file to https://netron.app/


