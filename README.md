MIT License

Copyright (c) 2025 Matthias Benitez

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

# Iris KNN Feature Selection & Decision Boundary Visualization

This project applies K-Nearest Neighbors (KNN) classification to the Iris dataset, comparing two approaches:

1. **Baseline Model** using all four Iris features.
2. **Feature-Selected Model** using only the top two features chosen using Mutual Information:
   - Petal Length (cm)
   - Petal Width (cm)

GridSearchCV is used in both models to determine the optimal K value.  
The feature-selected model is then visualized in a 2D decision boundary plot, with training and testing samples clearly distinguished.

## Key Results
| Model | Best K | Test Accuracy |
|------|-------|---------------|
| Baseline (All 4 features) | **7** | **0.947** |
| Feature-Selected (2 features) | **10** | **0.921** |

## Visualization
The final plot includes:
- Pastel decision regions for each predicted class
- Train samples as circles
- Test samples as squares with black outlines
- Colors:
  - **Purple** = Setosa
  - **Yellow** = Versicolor
  - **Teal** = Virginica

## Files
- `iris_knn_feature_selection.ipynb` – full code and visualizations
- `LICENSE` – MIT License

---

© 2025 **Matthias Benitez** — Licensed under the **MIT License**
