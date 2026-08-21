# Fashion MNIST Regularization Comparison

[![TensorFlow](https://img.shields.io/badge/TensorFlow-2.x-FF6F00?style=for-the-badge&logo=tensorflow)](https://www.tensorflow.org/)
[![Keras](https://img.shields.io/badge/Keras-2.x-D00000?style=for-the-badge&logo=keras)](https://keras.io/)
[![Python](https://img.shields.io/badge/Python-3.8+-3776AB?style=for-the-badge&logo=python)](https://www.python.org/)
[![License](https://img.shields.io/badge/License-MIT-yellow.svg?style=for-the-badge)](https://opensource.org/licenses/MIT)

##  Overview
This project compares different **regularization techniques** (L1, L2, and Dropout) on a **CNN** for **Fashion MNIST** classification, demonstrating how each method affects model performance and generalization.

##  Techniques Compared
| Technique | Description | Implementation |
|-----------|-------------|----------------|
| **Base Model** | No regularization | Standard CNN |
| **L1 Regularization** | L1 penalty for sparsity | `kernel_regularizer=l1(0.001)` |
| **L2 Regularization** | L2 penalty to prevent large weights | `kernel_regularizer=l2(0.001)` |
| **Dropout** | Randomly drops neurons during training | `layers.Dropout(0.5)` |

##  Model Architecture
Input (28, 28, 1) → Conv2D(32) → MaxPool → Conv2D(64) → MaxPool → Conv2D(128) → Conv2D(128) → Flatten → Dense(128) → Dense(10)



##  Results
| Model | Test Accuracy | Test Loss |
|-------|---------------|-----------|
| Base Model | 91.27% | 0.2443 |
| L1 Regularization | 90.34% | 0.2740 |
| L2 Regularization | 90.91% | 0.2618 |
| Dropout (0.5) | **91.71%** | **0.2398** |

##  Installation & Usage

git clone https://github.com/yourusername/fashion-mnist-regularization-comparison.git
cd fashion-mnist-regularization-comparison
pip install -r requirements.txt
python fashion_mnist_regularization.py
 Dependencies

tensorflow>=2.0.0
numpy>=1.19.0
matplotlib>=3.0.0
 License
MIT License - Copyright (c)  Vaibhav V Poojary

 Acknowledgments
Zalando Research for Fashion MNIST dataset

TensorFlow and Keras teams

Happy Learning!

LICENSE (MIT)
MIT License

Copyright (c)  Vaibhav V Poojary

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.

 requirements.txt
tensorflow>=2.0.0
numpy>=1.19.0
matplotlib>=3.0.0
