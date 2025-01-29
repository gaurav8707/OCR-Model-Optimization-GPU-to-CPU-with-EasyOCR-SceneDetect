# 🚀 Efficient OCR on CPU with EasyOCR & SceneDetect

## 📌 Project Overview
This project focuses on **optimizing a GPU-based OCR model to efficiently run on a CPU**. The optimization process involves:
- Selecting **EasyOCR** as the OCR engine.
- **Quantizing the model** to reduce computation overhead.
- **Integrating SceneDetect** for intelligent scene segmentation.
- **Testing on a dataset:** The lyrics of the song *"Sunroof"*.
- **Song Link:** [Sunroof - YouTube](https://www.youtube.com/watch?v=cWUt8UZunOE)

## 🎯 Goals
- ✅ Convert a **GPU-dependent OCR model** to run efficiently on CPU.
- ✅ Improve **execution speed** by **quantization & scene-based processing**.
- ✅ Evaluate **performance improvements** with execution time & FPS comparisons.

---

## 🔧 Installation & Setup
### 1️⃣ Clone the Repository
```sh
 git clone https://github.com/yourusername/Efficient-OCR-CPU.git
 cd Efficient-OCR-CPU
```

### 2️⃣ Install Dependencies
```sh
pip install easyocr opencv-python numpy scenedetect torch torchvision torchaudio
```

### 3️⃣ Quantize the OCR Model
```sh
python scripts/quantize_model.py
```

### 4️⃣ Run Scene Detection & OCR
```sh
python scripts/scenedetect.py --input video.mp4
python scripts/ocr_inference.py --input frames/
```

---

## 🚀 Performance Comparison
### 📊 **Execution Time (Lower is Better)**
| Setup                        | Execution Time (s) |
|------------------------------|--------------------|
| **GPU-based OCR**            | ❌ Not optimized  |
| **CPU-based OCR**            | ⏳ 2000+ sec      |
| **Quantized CPU + SceneDetect** | 🚀 151.40 sec  |

### 🎥 **FPS (Higher is Better)**
| Setup                        | FPS  |
|------------------------------|------|
| **GPU-based OCR**            | ❌ Not tested |
| **CPU-based OCR**            | ⏳ ~2 FPS     |
| **Quantized CPU + SceneDetect** | 🚀 **25 FPS** |

---

## 🤝 Contributing
Feel free to open an issue or a pull request if you want to improve this project. Contributions are welcome! 🚀
