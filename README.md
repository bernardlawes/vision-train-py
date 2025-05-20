
---

## 🧪 `vision-train-py/README.md`

```markdown
# 🧠 Vision Train and Eval (Python)

This repository contains tools, scripts, and configs for training and exporting object detection models using modern frameworks like YOLOv8, YOLO-NAS, RT-DETR, and Grounding DINO.

---

## 📁 Key Structure

| Folder         | Purpose |
|----------------|---------|
| `yolo/`        | YOLOv8 training and export |
| `transformers/`| RT-DETR, Grounding DINO training pipelines |
| `deployment/`  | Export scripts: ONNX, TFLite, TorchScript |
| `notebooks/`   | Colab-compatible demo notebooks |
| `tools/`       | Dataset converters, evaluators, and visualization |
| `datasets/`    | Training data (external or symlinked) |
| `models/`      | Exported model files (.pt, .onnx) |

---

## 🚀 Quickstart (YOLOv8)

```bash
pip install -r requirements.txt
python yolo/train.py --config yolo/config.yaml
python deployment/export_onnx.py --weights runs/train/weights/best.pt
```

## 🧠 Goals
Easy training of object detection models on custom datasets

Reliable export formats for deployment (ONNX, TFLite, TorchScript)

Full integration with C++ runtime via vision-common