# Image to GIF Creator (Python)

## 📌 Project Overview

This project is a simple Python script that converts multiple images into a single animated GIF. It uses the **imageio** library to read image files and combine them into a looping GIF animation.

This project is useful for beginners learning about image processing, file handling, and working with external Python libraries.

---

## 🎯 Features

* Reads multiple image files
* Combines images into an animated GIF
* Controls frame duration
* Supports infinite looping
* Lightweight and easy to use

---

## 🛠️ Technologies Used

* **Python 3**
* **imageio (v3)** library

---

## 📂 Project Structure

```
image_to_gif/
│
├── gif_creator.py      # Main Python script
├── download.jpg        # Input image 1
├── download1.jpg       # Input image 2
└── team.gif             # Output GIF file
```

---

## ▶️ How the Code Works

1. A list of image filenames is defined
2. Each image is read using `imageio.imread()`
3. Images are stored in a list
4. The list is written to a GIF file using `imageio.imwrite()`

---

## 🧾 Python Code

```python
import imageio.v3 as iio

filenames = ['download.jpg', 'download1.jpg']
images = []

for filename in filenames:
    images.append(iio.imread(filename))

iio.imwrite('team.gif', images, duration=500, loop=0)
```

---

## ▶️ How to Run the Project

### Step 1: Install Required Library

```bash
pip install imageio
```

### Step 2: Place Images

Ensure the image files (`download.jpg`, `download1.jpg`) are in the same folder as the script.

### Step 3: Run the Script

```bash
python gif_creator.py
```

### Step 4: Output

A GIF file named **team.gif** will be created in the same directory.

---

## ⚙️ Parameters Explained

* **duration=500** → Time each frame is shown (in milliseconds)
* **loop=0** → GIF loops infinitely

---

## 👤 Author

**Satya Thakur**
