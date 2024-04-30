
# HandWriting Based Author Identification

This project aims to predict the author of a handwritten document by analyzing the handwriting characteristics. The model utilizes two machine learning algorithms: Random Forest Classifier and Logistic Regression. After analyzing the results of both, Random Forest Classifier seems to be more suitable. It gives an accuracy of **87%** on training data and **84%** on testing data.

## Requirements

- **Python 3.x**
- **scikit-learn**
- **numpy**
- **pandas**
- **matplotlib**
- **os**
- **pickle**
- **Jupyter Notebook** (optional, for running the provided example notebook)

## Components

### Data Collection
Collect a dataset consisting of handwritten documents along with their corresponding authors. Ensure that the documents are scanned or digitized in a suitable format for analysis. For this purpose, the HandWritten Notes by Harry and MandarTule are used.

### Data Preprocessing
Preprocess the collected data to extract relevant features from the handwriting samples. This may include feature extraction techniques such as:


- Load image using OpenCV (cv2.imread()).
- Convert to grayscale, apply median blur, and threshold for noise reduction.
- Vertically crop text region and extract characters.
- Extract texture patches for local texture characteristics.
### Data Augmentation
To enhance the diversity of the dataset and improve model generalization, consider applying data augmentation techniques such as:

- Rotating the images slightly
- Adding noise to simulate variations in writing styles
- Flipping the images horizontally

### Model training
Train the Random Forest Classifier and Logistic Regression models using the preprocessed data. Split the dataset into training and testing sets to evaluate the performance of the models.

### Model Evaluation
Evaluate the performance of the trained models using appropriate evaluation metrics such as accuracy, precision, recall, and F1-score.

### Prediction
Use the trained models to predict the author of handwritten documents. Since Random Forest Classifier gave better accuracy, so it is used.

## Instruction to Usage

Run the **Prediction.ipynb** file and give the path of the Image whose HandWriting is to be specified. You can also use the images given in **Test_Images** to test the model.

## Deployment

To use the project, run the following command in the folder where you want to get the project.

```bash
  git clone git@github.com:anamfatima1304/HandWriting_Based_Author_Identification.git
```
Now play around with the model and enjoy.


## Acknowledgements

Special Thanks to codewithharry and mandartule for providing free HandWritten Notes that were valuable in creating the dataset.

 - [Notes By Harry](https://www.codewithharry.com/notes/)
 - [Notes By MandarTule](https://github.com/mandartule/Apna-College-AlphaBatch-DSA-JAVA/blob/main/Java%201.pdf)


## Contributing

Contributions are always welcome!

Find out an Error or give any suggestion to improve the project.

If you want to add any new features, make a pull request.

ThankYou for your attention.

**Happy Coding**
