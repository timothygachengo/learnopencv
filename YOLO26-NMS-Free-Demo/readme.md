# YOLO26 NMS-Free ONNX Inference

This folder contains a minimal example of running **YOLO26** (End-to-End) using **ONNX Runtime**.

Unlike traditional YOLO models that require complex post-processing (Non-Maximum Suppression), YOLO26 outputs a `[1, 300, 6]` tensor directly. This means the model has already selected the best detections for us.

### 🖼️ Result Preview
![YOLO26 Detection Result](YOLO26_Test_image_output.png)
*(The model directly outputs these boxes without NMS)*

---

## 📂 File Overview

* **`NMS_Free_Inference_with_YOLO26.ipynb`**: The main notebook. It loads the ONNX model, pre-processes the image, and visualizes the specific output format.
* **`Person_Dog.png`**: The raw input image used for testing (with class labels).
* **`YOLO26_Test_image.png`**: The raw input image used for testing.
* **YOLO26_Test_image.png**: Side-by-side comparison showing the original input (left) and the YOLO26 detections (right).

---

