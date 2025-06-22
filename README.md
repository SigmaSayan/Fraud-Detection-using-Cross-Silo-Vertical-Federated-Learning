# 🔐 Fraud Detection using Cross-Silo Vertical Federated Learning

This project implements a **PyTorch-based vertical federated learning (VFL)** system to detect fraudulent transactions without sharing raw data across institutions. Each party owns distinct feature sets for the same users, ensuring data privacy throughout the training process.

---

## 📁 Datasets
The model is trained on three vertically partitioned curated datasets:

- [`dataset1_train.csv`](https://drive.google.com/file/d/1SFsUuZN95avpr0n4FgwErQKzb6xTFJel/view?usp=sharing)  
- [`dataset2_train.csv`](https://drive.google.com/file/d/1lv6GXYwpnT9S5hzguG_e4KD7fHQxqepm/view?usp=sharing)  
- [`dataset3_train.csv`](https://drive.google.com/file/d/1SKK3qRuE0SvByO3XllabyrDzz1g9eWNm/view?usp=sharing)  

Each dataset contributes non-overlapping features, simulating real-world data silos.

---

## ⚙️ Project Highlights
- Built entirely using **PyTorch** — no external FL libraries  
- Custom federated training loop tailored for vertically split data  
- Secure architecture with no data leakage between silos  
- Target variable: `is_fraud` (binary classification)

---

## 📊 Evaluation Results
Achieved solid performance under constrained resources:

- ✅ **Test Accuracy**: 97.78%  
- ✅ **ROC-AUC Score**: 0.6070  

*Note: Precision and Recall were lower due to limited compute and GPU access, restricting training to ~10 epochs per round.*

---

## 🚀 How to Run
1. Place all three training datasets in your project directory  
2. Launch and run `Fraud_Detection_using_FL.ipynb` in Jupyter  
3. Follow the training and evaluation flow in the notebook cells

---

## 🎯 Objective
To demonstrate fraud detection across data silos using vertical federated learning, focusing on **model utility, data confidentiality, and real-world compute constraints**.

---

## ✍️ Author

**Sayan Das**  
*B.Tech + M.Tech in Mechanical & Financial Engineering*  
*Indian Institute of Technology, Kharagpur (IIT Kharagpur)*

---

