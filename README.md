README - Road Safety Classification Project
===========================================

This project is split into two main parts:
1. Image Preprocessing using OpenCV (CVIP)
2. Model Training and Testing

---

USAGE
-----

1. **Image Preprocessing (CVIP Part)**

To run the image processing module:
> python project_imageprocessingCVIP.py

This script applies computer vision techniques to prepare the dataset for model training.

---

2. **Model Training and Prediction**

To train the model and test it on a sample image, use:
> python project_model_training.py --csv_path output/road_safety_dataset.csv --test_image ./test_images/test_image.png --output_dir ./output --epochs 10

- `--csv_path` : Path to the dataset CSV file
- `--test_image` : Path to an image for testing
- `--output_dir` : Directory where results will be saved
- `--epochs` : Number of training epochs

---

3. **Jupyter Notebook Alternative**

We have also provided a Jupyter Notebook with the same logic. You can run the notebook step-by-step to execute both image processing and model training in an interactive environment.

---

4. **Web UI for Model Inference**

To launch the web-based UI built on top of the trained model, you can upload test images in test_images folder: 

```bash
cd road_safety_app
pip install -r requirements.txt
python3 app.py
pause
