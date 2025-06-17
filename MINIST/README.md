# MNIST Digit Classification

This project demonstrates handwritten digit classification using the famous **MNIST dataset**. The dataset contains grayscale images of handwritten digits ranging from 0 to 9.

## Objective

To build and train a neural network that can accurately classify digits in the MNIST dataset.

## Technologies Used

- Python
- TensorFlow / Keras
- NumPy
- Matplotlib
- Scikit-learn (for evaluation metrics)

  
## Model Training Summary
Dataset: MNIST (Handwritten Digit Classification)

Model: Multi-Layer Perceptron (MLP)

- Epochs: 5

- Final Training Accuracy: 98.88%

- Final Testing Accuracy: 97.56%

- Loss: Decreased steadily from 0.4971 to 0.0794

The model shows excellent generalization with minimal overfitting. Further improvements can include hyperparameter tuning or training for more epochs to achieve even higher accuracy.

<img width="731" alt="Screenshot 2025-06-18 at 4 39 43 AM" src="https://github.com/user-attachments/assets/f145e285-64b2-4681-a804-846a55a1b98c" />


## Steps Covered in the Notebook

1. **Data Loading**  
   Loaded the MNIST dataset directly using Keras datasets.

2. **Data Preprocessing**  
   - Normalized the pixel values to the range [0,1].
   - One-hot encoded the target labels.

3. **Model Building**  
   - Built a simple feedforward neural network (fully connected layers).
   - Used ReLU activation for hidden layers and Softmax for the output layer.

4. **Model Training**  
   - Compiled using categorical crossentropy loss.
   - Trained with an optimizer such as Adam.
   - Evaluated on validation and test sets.

5. **Evaluation & Results**  
   - Calculated accuracy on the test set.
   - Plotted training and validation accuracy/loss curves.
   - Displayed predictions and sample images.

6. **Conclusion**  
   - The model achieved a high accuracy suitable for basic digit recognition tasks.

## Sample Output

- **Test Accuracy**: ~98% (exact value in the notebook)
- Training and validation plots available.

## Requirements

Install the following packages:

```bash
pip install numpy matplotlib tensorflow scikit-learn

