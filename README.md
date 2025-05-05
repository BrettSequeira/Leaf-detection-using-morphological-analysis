# 🍃 Leaf Classifier - Mango, Banana, Maple

This project is a simple image-based leaf classification system using Python, OpenCV, and scikit-learn. It distinguishes between mango, banana, and maple leaves using basic shape-based features and a Random Forest classifier.

## 🧠 How It Works

- Uses OpenCV to extract shape-based features from leaf images.
- Trains a Random Forest classifier on the extracted features.
- Predicts the type of leaf based on an input image.

## 🔍 Features Used
- Contour Area
- Perimeter
- Aspect Ratio
- Extent (Area / Bounding box area)
- Solidity (Area / Convex Hull area)

## 📁 Folder Structure

```
project-root/
│
├── dataset/
│   ├── mango/
│   ├── banana/
│   └── maple/
│
├── test3.jpg         # Example test image
├── leaf_classifier.py
└── README.md
```

## 🚀 Getting Started

### 1. Install Requirements

```bash
pip install opencv-python numpy scikit-learn
```

### 2. Add Dataset

Place images of each leaf type in the corresponding subfolders inside the `dataset/` directory:
- `dataset/mango`
- `dataset/banana`
- `dataset/maple`

Make sure images are clear and focused on the leaf.

### 3. Run the Classifier

Edit the script if needed and run:

```bash
python leaf_classifier.py
```

You should see a prediction like:
```
Prediction: Mango Leaf 🥭
```

### 🔄 Add More Leaf Types?

You can add new leaf types by:
1. Adding a new folder under `dataset/`
2. Updating the `load_dataset()` and `predict_leaf()` functions to include the new class

## 🛠 Future Improvements
- Add more robust features (color, texture)
- Use deep learning (CNN) for higher accuracy
- Build a simple GUI with Tkinter or a web app

## 📜 License

This project is free to use for educational and research purposes.

## 👥 Team Members

- **Brett Dylan Sequeira** (USN: 4SO22CD013)
- **Lionel Rosario** (USN: 4S022CD028)
- **Trisha Veigas** (USN: 4S022CD060)
