# Keybr Score Prediction Model

A machine learning model that reverse-engineers the scoring algorithm used by keybr.com to predict typing test scores based on Words Per Minute (WPM) and accuracy.

## Project Overview

I was practicing typing on keybr.com and got curious about how their scoring system worked. So I collected my typing test data and built a machine learning model to figure out their scoring calculation. 

## Results

- **Model**: Ridge Regression with 5th-degree polynomial features
- **Accuracy**: R² = 0.980
- **Error Rate**: 6.2% average prediction error
- **Validation MAE**: 469 points

## Try It Yourself

```python
# Predict your keybr score and percent error
actual_score = 4107  # change to your actual score
wmp = 95.4  # change to your actual wpm
accuracy = 95.93  # change to your actual accuracy
predicted_score = predict_score(wpm, accuracy)
print(f"Predicted Score: {predicted_score:.0f}")
percent_error = ((abs(predicted_score - actual_score)) / actual_score) * 100
print(f"Percent Error: {percent_error:.2f}%")
