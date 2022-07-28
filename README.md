# stock_price_forecasting

File berisi perbandingan antara LGBM, CatBoost, dan XGBoost. Data didapat dari Yahoo Finance menggunakan `yfinance` dari tanggal 01/01/1992 sampai tanggal 01/01/2022 dengan jumlah 7558 data.


## Distribusi data
![alt text](https://github.com/yanuarkholik/stock_price_forecasting/blob/main/image/data_dist1.png) ![alt boxplot1](https://github.com/yanuarkholik/stock_price_forecasting/blob/main/image/boxplot1.png)

Distribusi data setelah transformasi

Distribusi leukoptik dan kurtosis yang tinggi (kurtosis=26), hal ini dikarenakan data memiliki banyak sekal outlier. Author terpaksa menghapus outlier karena outlier handling kurang berpengaruh terhadap data.


![alt text](https://github.com/yanuarkholik/stock_price_forecasting/blob/main/image/data_dist2.png)
![alt text](https://github.com/yanuarkholik/stock_price_forecasting/blob/main/image/boxplot2.png)

Distribusi data setelah perghapusan outlier.

Masih terdapat sedikit outlier yang tersisa namun tidak terlalu berpengaruh terhadap kurtosis (kurotosis=0.75).

## Hasil
| | LGBM | CatBoost | XGBoost | 
| ----------- | ----------- | ----------- | ----------- |
| RMSE | 0.02599 | 0.030027 | 0.030026 | 
| MAE | 0.02158 | 0.02441 | 0.02441 |
| sMAPE | 145.82 | 149.47| 149.65 |
