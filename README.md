
# Random Forest for Digit Classification (MNIST Dataset)

## Project Description
This project demonstrates the application of the Random Forest algorithm for handwritten digit classification using the MNIST dataset. The goal is to build and evaluate a Random Forest model to classify digits and analyze its performance through error metrics and visualizations.

## Features
- Implements a Random Forest with 50 trees for classification.
- Evaluates model performance with OOB (Out-Of-Bag) error and confusion matrices.
- Analyzes the most significant pixels (features) contributing to classification decisions.
- Compares Random Forest performance to simpler models.

## Included Files
1. **Code**:
   - `random_forest.Rmd`: R Markdown file containing the implementation of the Random Forest algorithm and analyses.
2. **Data**:
   - `digit_train.csv` and `digit_test.csv`: Training and test datasets for digit classification.

## Dataset Description
- The MNIST dataset comprises 60,000 training examples and 10,000 test examples of handwritten digits, normalized and centered on 28x28-pixel grayscale images.
- Each row in the dataset represents one image, with:
  - `digit`: The class label for the digit.
  - `X1` to `X784`: Grayscale values for each pixel (flattened).

## Requirements
- **R**: Version 4.0 or higher
- Required Libraries:
  - `randomForest`
  - `rpart`
  - `rpart.plot`
  - `plotmo`
  - `rattle`

Install dependencies:
```R
install.packages(c("randomForest", "rpart", "rpart.plot", "plotmo", "rattle"))
```

## Usage
1. Clone this repository:
   ```bash
   git clone https://github.com/rmodregoe/mnist-random-forest-classification.git
   ```
2. Load the R Markdown file (`random_forest.Rmd`) in RStudio.
3. Run the analysis step-by-step or knit the document for a comprehensive report.

## Results
- **Model Performance**:
  - OOB error rate: ~4.12% with 50 trees.
  - Confusion matrices and error rates for each digit.
- **Feature Importance**:
  - Identifies the most significant pixels for digit classification.
- **Visualization**:
  - Displays example digits and highlights misclassified cases.

## License
This project is licensed under the [MIT License](LICENSE).

## Contact
Created by Ricardo Modrego. For questions or feedback, contact me at [r.modrego.e@gmail.com](mailto:r.modrego.e@gmail.com).
