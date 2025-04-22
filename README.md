## Heart Disease Prediction using Neural Networks and Optimizer Comparison
This project explores the performance of different optimization techniques for training a neural network on a heart disease risk prediction dataset. It compares modern evolutionary algorithms with traditional optimizers in terms of classification accuracy and training loss.

## 📊 Dataset
The dataset used is `heart_disease_risk_dataset_earlymed.csv`, which includes 18 input features and a binary target variable indicating heart disease risk (`0 = No Risk`, `1 = Risk`).

## 🛠️ Project Structure
├── cheetah_optimizer.ipynb # Uses the Cheetah Optimizer (nature-inspired) ├── genetic_algorithm.ipynb # Uses a Genetic Algorithm for optimization ├── keras_optimizers.ipynb # Uses Adam, SGD, and RMSprop (Keras built-ins) ├── heart_disease_risk_dataset_earlymed.csv ├── README.md # Project summary


## ⚙️ Neural Network Architecture
A consistent feedforward neural network is used for all experiments:
- Input layer with 18 features
- Hidden Layers:
  - Dense(64), ReLU + Dropout(0.3)
  - Dense(32), ReLU
  - Dense(16), ReLU
- Output Layer: Dense(1), Sigmoid (binary classification)

## 🧪 Optimization Techniques Compared

| Optimizer          | Type              | Notes                              |
|--------------------|-------------------|-------------------------------------|
| **Cheetah Optimizer** | Nature-inspired | Exploits swarm intelligence for search |
| **Genetic Algorithm** | Evolutionary     | Based on selection, crossover, mutation |
| **Adam**            | Gradient-based    | Adaptive learning rate, widely used |
| **SGD**             | Gradient-based    | Classic stochastic gradient descent |
| **RMSprop**         | Gradient-based    | Adaptive gradient method with momentum |

## 📈 Evaluation Metrics
- **Accuracy**: Proportion of correct predictions
- **Loss**: Binary Cross-Entropy Loss
- **Confusion Matrix** (optional)
- **Training Curves**: Accuracy and loss vs. epochs/generations

## 🧠 Key Highlights

- ✅ Cheetah and Genetic optimizers are implemented from scratch in Python
- ✅ Accuracy/loss tracked across epochs/generations
- ✅ All optimizers tested under the same network conditions
- ✅ Visual comparisons using `matplotlib`, `tabulate`, `seaborn`
- ✅ Efficient, scalable, and educational

## 📌 How to Run

1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/heart-optimizer-comparison.git
   cd heart-optimizer-comparison
2. Open any notebook in Jupyter or Google Colab.

3. Run cells from top to bottom. Results will appear as tables and plots.

## 📚 Dependencies
pip install numpy pandas matplotlib seaborn scikit-learn tabulate tensorflow
