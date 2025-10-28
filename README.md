# 🧠 Deep Learning Polynomial Regression

Bu loyiha Keras yordamida yaratilgan oddiy sun’iy neyron tarmoq asosida kvadrat regressiyani bashorat qiladi.

## 📁 Fayllar:
- `model_training.ipynb` — asosiy kod
- `deep_model.h5` — tayyor o‘qitilgan model
- `model_structure.png` — model tuzilmasi rasmi

## 🚀 Foydalanish:
```python
from tensorflow.keras.models import load_model
model = load_model("deep_model.h5", compile=False)
model.compile(optimizer='adam', loss='mse')
print(model.predict([[6.0]]))
