# Inference_with_OpenVINO_Execution_Provider

This weekend I decided to play around with OpenVINO™ Execution Provider for ONNX Runtime on Google Colab. My goal was to run inference on a PyTorch MobileNet v2 image classification model from Torchvision with just the one simple change required to use OpenVINO™ Execution Provider with ONNX Runtime.

Check out the video below for yourself to see how I ran inferencing using OpenVINO™ Execution Provider for ONNX Runtime on Google Colab.

Try the notebook out for yourself on Google Colab: 
https://github.com/R-Mahmoudi/Inference_with_OpenVINO_Execution_Provider/blob/main/Inference_with_OpenVINO_Execution_Provider.ipynb


PyPi Link: https://pypi.org/project/onnxruntime-openvino/


1) pip install onnxruntime-openvino

2) import onnxruntime

3) session = onnxruntime.InferenceSession("model.onnx", providers=['OpenVINOExecutionProvider'], provider_options=[{'device_type' : '<device>'}])

4) Run inference using ONNX Runtime API
