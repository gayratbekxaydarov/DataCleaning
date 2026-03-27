# 🩺 Diabetes Data Preprocessing & Analysis (KNN Imputation & PCA)

Ushbu loyiha diabetga oid ma'lumotlar to'plamini (dataset) tozalash, yetishmayotgan qiymatlarni to'ldirish va vizuallashtirish uchun ishlab chiqilgan. Loyihada asosiy e'tibor ma'lumotlar sifatini oshirishga va o'lchovni kamaytirishga (dimensionality reduction) qaratilgan.

---

## 🚀 Loyihaning asosiy funksiyalari

Loyihada ma'lumotlar bilan ishlashning to'liq sikli amalga oshirilgan:

1.  **KNN Imputation (0-larni to'ldirish):** Datasetdagi `0` qiymatlarni shunchaki o'chirmasdan, **K-Nearest Neighbors** algoritmi yordamida eng yaqin qo'shni qatorlarning o'rtacha qiymati bilan aqlli ravishda to'ldiradi.
2.  **Korrelyatsiya tahlili:** Ustunlar orasidagi bog'liqlikni hisoblab, ma'lumotlar modelga xalaqit bermasligi uchun ortiqcha yoki bog'liqligi juda yuqori ustunlarni aniqlaydi.
3.  **Outlier Detection (Chetlanishlarni topish):** **IQR (Interquartile Range)** usuli yordamida statistik xatolarni va anomal qiymatlarni topadi.
4.  **PCA (Principal Component Analysis):** Ma'lumotlarning o'lchamini 2 ta asosiy komponentaga tushiradi va natijani **Matplotlib** orqali vizuallashtiradi.

---

## 🛠 Kerak bo'ladigan kutubxonalar
* **Python 3.x**
* **NumPy & Pandas:** Ma'lumotlarni qayta ishlash uchun.
* **Matplotlib:** Grafiklar va vizuallashtirish uchun.
* **Scikit-learn:** PCA algoritmi uchun.
---
## 📊 Kod qanday ishlaydi?

### 1. Ma'lumotlarni tozalash (Imputation)
Kod har bir nol qiymatga ega bo'lgan qator uchun boshqa barcha qatorlar bilan Evklid masofasini hisoblaydi va eng yaqin K ta qo'shnini topadi:
r = sum((x[i] - mean(x)) * (y[i] - mean(y))) / (sqrt(sum((x[i] - mean(x))**2 * (y[i] - mean(y))**2 )))  

### 2. PCA Vizuallash
8 ta ustundan iborat murakkab ma'lumotlar to'plamini 2D tekislikka o'tkazadi. Bu ma'lumotlarning umumiy strukturasini va klassterlanishini ko'rish imkonini beradi.
Kerakli kutubxonalarni o'rnatish:
    pip install numpy pandas matplotlib scikit-learn
Skriptni ishga tushurish:
    python main.py
-------------------------------------------------------------------
🩺 Diabetes Data Preprocessing & Analysis (KNN Imputation & PCA)This project is designed to clean, impute missing values, and visualize a diabetes-related dataset. The primary focus is on enhancing data quality and performing dimensionality reduction to better understand the underlying patterns.

🚀 Key Features
The project implements a full data processing pipeline:
  KNN Imputation: Instead of simply deleting rows with 0 values, the K-Nearest Neighbors algorithm is used to intelligently fill gaps with the mean of the most similar data points.
  Correlation Analysis: Calculates relationships between features to identify redundant or highly correlated columns that might hinder model performance.
  Outlier Detection: Uses the IQR (Interquartile Range) method to detect statistical anomalies and extreme values.
  PCA (Principal Component Analysis): Reduces the dataset from 8 dimensions down to 2 principal components for effective visualization using Matplotlib.
🛠 Prerequisites:
  Python 3.xNumPy & Pandas: For data manipulation.
  Matplotlib: For plotting and visualization.
  Scikit-learn: For the PCA algorithm.
How It Works:
  Imputation: The code calculates the Euclidean distance between rows to find the K nearest neighbors for every missing value.
  PCA Visualization: Transforms a complex 8-column dataset into a 2D plane, allowing for clear observation of data clusters and structure.
Installation:
    pip install numpy pandas matplotlib scikit-learn
Run the script:
    python main.py
---------------------------------------------------------------------
🩺 糖尿病データの分析と前処理 (KNN補完とPCA)
このプロジェクトは、糖尿病データセットのクリーニング、欠損値の補完、および可視化を行うために開発されました。データの品質向上と次元削減（Dimensionality Reduction）に重点を置いています。
主な機能
このプロジェクトでは、以下のデータ処理パイプラインを実装しています：

KNN補完 (KNN Imputation): 0（欠損値）を単に削除するのではなく、K近傍法アルゴリズムを使用して、最も近い近傍値の平均でスマートに補完します。

相関分析: 特徴量間の相関を計算し、モデルの精度に影響を与える可能性のある冗長な列を特定します。

外れ値検出: IQR (四分位範囲) 法を用いて、統計的な異常値や外れ値を検出します。

主成分分析 (PCA): 8つの特徴量を持つデータを2次元に圧縮し、Matplotlibを使用して視覚化します。

必要ライブラリ

Python 3.x

NumPy & Pandas: データ操作用。

Matplotlib: グラフ作成および可視化用。

Scikit-learn: PCAアルゴリズム用。

仕組み:
データ補完: 各欠損値に対して、他のデータ行とのユークリッド距離を計算し、最も近い $K$ 個のデータを特定します。PCA可視化: 複雑な8次元データを2次元平面に変換することで、データの構造やクラスタリングを容易に確認できるようにします。

インストール方法:
    pip install numpy pandas matplotlib scikit-learn
実行方法:
    python main.py

   ```bash
   git clone [https://github.com/foydalanuvchi_nomi/diabetes-data-preprocessing.git](https://github.com/foydalanuvchi_nomi/diabetes-data-preprocessing.git)
