# Keybr Score Prediction Model

A machine learning model that reverse-engineers the scoring algorithm used by keybr.com to predict typing test scores based on Words Per Minute (WPM) and accuracy.

## Project Overview

I was practicing typing on keybr.com and got curious about how their mysterious scoring system worked. So I collected my typing test data and built a machine learning model to figure out their scoring calculation. Turns out it's pretty complex!

## Results

- **Model**: Ridge Regression with 5th-degree polynomial features
- **Accuracy**: R² = 0.980
- **Error Rate**: 6.2% average prediction error
- **Validation MAE**: 469 points

## Try It Yourself

```python
# Predict your keybr score
predicted_score = predict_score(wpm=95.4, accuracy=95.93)
print(f"Predicted Score: {predicted_score:.0f}")
