# Road Sign Detection using Convolutional Neural Networks (CNN)

## Description

Road sign detection and classification play a crucial role in autonomous driving systems. This project utilises TensorFlow and Keras to create a CNN model that can classify road signs into various categories.

## Dataset Directory Structure
Ensure the dataset is organised in the following directory structure:

```
ROAD-SIGN-DETECTION/
│
├── traffic Data/
│   ├── TEST/
│   ├── TRAIN/
│   └── VAL/
│
├── Classifying Road Signs.ipynb
├── labels.csv
├── model.h5
├── README.md
└── Splitting Dataset.ipynb
```

In this structure:
- The `traffic Data` directory contains subdirectories `TEST`, `TRAIN`, and `VAL`, which store the testing, training, and validation datasets respectively.
- `Classifying Road Signs.ipynb` is a Jupyter Notebook containing code for classifying road signs.
- `labels.csv` is a CSV file containing labels for the images in the dataset.
- `model.h5` is the trained model saved in HDF5 format.
- `README.md` is the readme file containing project documentation and instructions.
- `Splitting Dataset.ipynb` is a Jupyter Notebook containing code for splitting the dataset into training and validation sets.

## Splitting Dataset
To split the dataset, you can use the `Splitting Dataset.ipynb` notebook. This notebook uses the `splitfolders` library to split the dataset into training and validation sets with specified ratios. 

## Dependencies
Ensure you have the following dependencies installed:
- TensorFlow
- matplotlib
- pandas
- numpy
- PIL

You can install these dependencies via pip:
```bash
pip install tensorflow matplotlib pandas numpy Pillow 
```

## Usage
1. **Clone the repository:**
```bash
git clone https://github.com/FunmiOlaitan/Road-Sign-Detection.git
cd Road-Sign-Detection
```

2. **Load and Analyze Dataset:**
   - The dataset is located in the `traffic_Data` directory.
   - Use the provided Python script to load and analyze the dataset, including class distribution and visualizations.

3. **Preprocessing:**
   - Images are preprocessed and augmented using the `ImageDataGenerator` from TensorFlow's Keras API.

4. **Build Custom Model:**
   - A custom CNN model is built using TensorFlow's Keras functional API. It consists of convolutional, max-pooling, flatten, dense, dropout, and softmax layers.

5. **Train the Model:**
   - The model is trained using the training data and validated using the validation data.
   - Training history (accuracy and loss) is visualised using Matplotlib.

6. **Save the Model:**
   - Once trained, the model is saved in the `.h5` format for future use.


## Customisation
You can customise the project by adjusting the following:
- Image dimensions and batch size for training.
- CNN model architecture and hyperparameters.
- Data augmentation techniques.
- Training epochs and learning rate.


## Acknowledgements
Special thanks to the creators of the `splitfolders` library for simplifying dataset splitting and to the authors of the various libraries used in this project.

## Support
For any issues or inquiries, feel free to open an issue in the repository. Your contributions and feedback are welcome to enhance the project further.

## Credits:

For any questions or issues, please contact the author at Funmilolaolaitan@yahoo.com