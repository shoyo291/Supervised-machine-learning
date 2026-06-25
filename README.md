# Supervised-machine-learning
# Titanic Survival Prediction

## Performance Comparison

| Model | Accuracy | Precision (Survived) | Recall (Survived) | F1-Score (Survived) |
|---------|----------|----------|----------|----------|
| Logistic Regression | 77.10% | - | - | - |
| k-Nearest Neighbors (KNN) | 75.95% | 0.80 | 0.63 | 0.70 |
| Random Forest | **79.01%** | **0.82** | **0.68** | **0.74** |

## Best Model: Random Forest

Random Forest achieved the highest performance across all metrics.

### Why Random Forest Performed Best

- **Ensemble Method**: Combines multiple decision trees, reducing overfitting and improving generalization.
- **Handles Feature Interactions**: Captures complex relationships such as the combined effect of gender and passenger class on survival.
- **Robust to Irrelevant Features**: Automatically reduces the impact of less informative features.

## Why the Other Models Fall Short

### Logistic Regression
- Achieved an accuracy of **77.10%**.
- Performs reasonably well because many survival patterns are approximately linear.
- Cannot capture complex non-linear interactions between features.

### k-Nearest Neighbors (KNN)
- Achieved an accuracy of **75.95%**.
- Sensitive to feature scaling and distance calculations.
- Performance may improve with better hyperparameter tuning (e.g., choosing a different value for *k*).

## Conclusion

Random Forest is the most suitable model for the Titanic survival prediction task, providing the best balance between accuracy, precision, recall, and F1-score.

Future improvements may include:
- Feature engineering (e.g., passenger titles, family size).
- Hyperparameter tuning.
- Cross-validation.
- Additional ensemble techniques.
