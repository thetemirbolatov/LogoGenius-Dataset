# 🎨 Logo Dataset by thetemirbolatov

> **5000+ уникальных логотипов для обучения нейросетей**
> Создано [@thetemirbolatov](https://github.com/thetemirbolatov)

---

## 📦 Что внутри

Архив содержит **5000+ PNG изображений** логотипов в разрешении **1024×1024 пикселей**.

```
logo_dataset.rar
├── 01_circles/          # Круги (200+ шт)
├── 02_triangles/        # Треугольники (200+ шт)
├── 03_squares/          # Квадраты (200+ шт)
├── 04_lines/            # Линии (200+ шт)
├── 05_stars/            # Звёзды (200+ шт)
├── 06_hexagons/         # Шестиугольники (200+ шт)
├── 07_abstract/         # Абстракция (200+ шт)
├── 08_dots/             # Точки (200+ шт)
├── 09_geometric_mix/    # Геометрический микс (200+ шт)
├── 10_minimal/          # Минимализм (200+ шт)
├── 11_gradients/        # Градиенты (200+ шт)
└── 12_tech/             # Tech стиль (200+ шт)
```

---

## 📊 Характеристики

| Параметр | Значение |
|----------|----------|
| Количество | 5000+ |
| Формат | PNG |
| Разрешение | 1024×1024 |
| Категорий | 12 |
| Размер архива | ~500 MB |

---

## 🎯 Для чего подходит

- Обучение GAN и VAE для генерации логотипов
- Классификация стилей логотипов
- Transfer Learning
- Data Augmentation
- Computer Vision проекты

---

## 🚀 Как использовать

### 1. Распаковать архив
```bash
unrar x logo_dataset.rar
# или
rar x logo_dataset.rar
```

### 2. Загрузить в Python
```python
from PIL import Image
import os

# Пройти по всем папкам
for folder in os.listdir("logo_dataset"):
    folder_path = os.path.join("logo_dataset", folder)
    if os.path.isdir(folder_path):
        for img_file in os.listdir(folder_path):
            img = Image.open(os.path.join(folder_path, img_file))
            # Ваш код обработки
```

### 3. Использовать для обучения
```python
import tensorflow as tf

# Создать датасет
dataset = tf.keras.preprocessing.image_dataset_from_directory(
    "logo_dataset",
    image_size=(64, 64),
    batch_size=32
)

# Обучить модель
model.fit(dataset, epochs=50)
```

---

## 📝 Лицензия

MIT License - можно использовать свободно в любых проектах.

---

## 👤 Автор

**Temirbolatov**

- GitHub: [@thetemirbolatov](https://github.com/thetemirbolatov)
- Hugging Face: [@thetemirbolatov](https://huggingface.co/thetemirbolatov)

---

## ⭐ Поддержка

Если датасет полезен, поставьте звезду ⭐ на GitHub!

```

---

## 📁 Что загрузить:

### Структура папок для GitHub:
```
LogoGenius-Dataset/
├── README.md
├── LICENSE
├── logo_dataset.rar        # Сам архив с PNG
└── models/                  # Папка с моделями (опционально)
    ├── LogoGenius_AI_v1.pkl
    └── LogoGenius_AI_v2_enhanced.pkl
```

### Структура для Hugging Face:
```
LogoGenius-Dataset/
├── README.md
├── dataset_card.md
├── data/
│   ├── 01_circles/
│   ├── 02_triangles/
│   └── ...
└── models/
```

---

## 🔗 Ссылки для публикации:

**GitHub:**
```
https://github.com/thetemirbolatov/LogoGenius-Dataset
```

**Hugging Face:**
```
https://huggingface.co/datasets/thetemirbolatov/LogoGenius-Dataset

Всё готово для публикации! 🚀
