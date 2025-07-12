# ML_Prediccion-del-Precio-Real-de-Productos-en-Amazon
**Autor:** Estefany Amesty

---

## Descripción del problema / Problem Description

**ES:**  
En muchas plataformas de comercio electrónico como Amazon, los productos se muestran con precios "con descuento" que a veces no reflejan un precio real coherente. Esto puede generar desconfianza en los usuarios y dificultar la estrategia de pricing.

Este proyecto tiene como objetivo desarrollar un modelo de Machine Learning que prediga el precio real de un producto basándose en sus características (precio con descuento, categoría, rating, etc.).

**EN:**  
On platforms like Amazon, the listed "discounted prices" often do not reflect a consistent or realistic base price. This affects user trust and makes pricing strategy harder.

This project aims to build a Machine Learning model to predict the actual (pre-discount) price of a product based on its features (discounted price, category, rating, etc.).

---

## Dataset

**ES:**  
El dataset contiene 1.465 productos extraídos de Amazon(Kaggle), con las siguientes columnas clave:

- `discounted_price`: precio con descuento (₹)
- `actual_price`: precio real (₹) [Target]
- `discount_percentage`: porcentaje de descuento (%)
- `rating`: puntuación media (de 1 a 5)
- `rating_count`: número de valoraciones
- `category`: categoría jerárquica (ej. "Electronics|TV")

**Tipo:** PUblico 
**Formato:** CSV  
**Acceso:** https://www.kaggle.com/datasets/ahmedsayed564/amazon-sales-dataset

**EN:**  
The dataset contains 1,465 Amazon products with these key features:

- `discounted_price` (₹)
- `actual_price` (₹) [Target]
- `discount_percentage` (%)
- `rating` (1 to 5)
- `rating_count`
- `category` (e.g., "Electronics|TV")

**Type:** Public
**Format:** CSV  
**Access:** https://www.kaggle.com/datasets/ahmedsayed564/amazon-sales-dataset

---

## Solución adoptada / Adopted Solution

**ES:**  
Se aplicó un enfoque supervisado de regresión. Se probaron tres modelos: `LinearRegression`, `RandomForestRegressor` y `GradientBoostingRegressor`.  
Tras una optimización con GridSearchCV, el modelo final (`GradientBoostingRegressor`) obtuvo:

- MAE: ₹234.49  
- RMSE: ₹918.79  
- R²: 0.9899

**EN:**  
We used a supervised regression approach and tested three models: `LinearRegression`, `RandomForestRegressor`, and `GradientBoostingRegressor`.  
After tuning with GridSearchCV, the final model (`GradientBoostingRegressor`) achieved:

- MAE: ₹234.49  
- RMSE: ₹918.79  
- R²: 0.9899


## Estructura del repositorio  
── src/                
    ├── data_sample/   
    ├── img/            
    ├── models/         
    ├── notebooks/     
    ├── utils/          
├── main.ipynb          
├── presentacion.pdf    
├── README.md           
