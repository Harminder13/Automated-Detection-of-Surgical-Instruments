---

# 🏥 **Automated Surgical Instrument Detection with YOLOv8 and YOLOv11**  

This project focuses on the **real-time detection and classification of surgical instruments** using advanced object detection models: **YOLOv8** and **YOLOv11**. Accurate identification and tracking of surgical instruments are essential for ensuring patient safety and improving operational efficiency in medical procedures. Traditional manual methods are prone to human error — our solution leverages state-of-the-art YOLO models to automate and enhance the process.

---

## 📌 **Motivation**
Surgical procedures rely on the precise identification and tracking of instruments to avoid complications and ensure procedural efficiency. Manual counting and verification can lead to human error, risking patient safety. The goal of this project is to develop a robust, real-time surgical tool detection system to automate this process and reduce the margin of error.

---

## 🚀 **Model Overview**
### 🔹 **YOLOv8**
- Implemented for initial testing and baseline comparison.  
- Achieved high true positive rates for most surgical instruments.  
- Challenges with distinguishing visually similar tools, particularly the **Straight Mayo Scissors** and **Curved Mayo Scissors** due to their similar profiles.  

### 🔹 **YOLOv11**
- Enhanced with **C3K2 blocks** and the **SPFF module** for better multi-scale feature extraction.  
- Achieved a mean F1-score of **0.98** across validation and test sets.  
- Strong generalization for tools like **Scalpel** and **Curved Mayo Scissors** with high recall and precision.  

---

## 📊 **Results**
### 🔥 YOLOv8 Performance:
- F1-Score: **0.96**  
- Mean Average Precision (mAP): **0.988**  

![YOLOv8 F1 Curve](./images/yolov8_f1_curve.png)  
![YOLOv8 Precision-Recall Curve](./images/yolov8_precision_recall.png)  

### 🌟 YOLOv11 Performance:
- F1-Score: **0.98**  
- Mean Average Precision (mAP): **0.991**  

![YOLOv11 F1 Curve](./images/yolov11_f1_curve.png)  
![YOLOv11 Precision-Recall Curve](./images/yolov11_precision_recall.png)  

---

## 🧪 **Challenges and Observations**
- **Class Confusion**: High similarity between Straight Mayo Scissors and Curved Mayo Scissors leads to misclassification.  
- **Lighting and Orientation**: Variations in lighting and instrument angles impact detection performance.  
- **Occlusions**: Overlapping instruments reduce detection accuracy in complex surgical environments.  

---

## 🔎 **Future Improvements**
✅ Fine-tune feature extraction to emphasize subtle geometric differences.  
✅ Introduce more diverse training data, including real-world surgical scenarios.  
✅ Adjust confidence thresholds and NMS (Non-Maximum Suppression) to improve recall.  

---

## 🎯 **Conclusion**
This project successfully demonstrates the potential of YOLO-based models for real-time surgical tool detection. With high mAP and F1 scores, the models show promise for real-world deployment in surgical environments — paving the way for improved accuracy, operational efficiency, and patient safety.

---

✨ **Feel free to explore the code and contribute!**  

---
