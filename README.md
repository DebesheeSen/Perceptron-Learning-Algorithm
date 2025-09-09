# Perceptron Decision Boundary Visualization  

This project implements the **Perceptron Learning Algorithm** and dynamically visualizes the evolution of its decision boundary during training.  

---

## ✨ Features  
- Implements a **basic perceptron classifier** from scratch using NumPy.  
- Updates the **decision boundary line** using Matplotlib.  
- Demonstrates how the perceptron gradually adjusts its weights to separate two classes.   

---

## 📊 How It Works  
1. **Dataset Generation**  
   - The example script generates random 2D points and assigns labels (`0` or `1`) based on the x-coordinate.  
   - You can replace this with your own dataset.  

2. **Perceptron Algorithm**  
   - Adds a bias term to each input.  
   - Initializes weights as ones.  
   - Iteratively updates weights:  
     $$ w \leftarrow w + \eta (y - \hat{y})x $$
     where $ \eta $ is the learning rate.  

3. **Decision Boundary**  
   - Computed from:  
     $$
     w_0 + w_1x + w_2y = 0 \quad \Rightarrow \quad y = -\frac{w_0 + w_1x}{w_2}
     $$
   - The separating line is updated on the plot.  

4. **Visualization**  
   - Blue and green dots represent the two classes.  
   - The red line is the **current decision boundary**.  
   - The plot title shows the **iteration number**.  

---

## 🚀 Usage  
Clone this repository and run the script:  

```bash
git clone https://github.com/yourusername/perceptron-learning-algorithm.git
cd perceptron-learning-algorithm
python perceptron.ipynb

