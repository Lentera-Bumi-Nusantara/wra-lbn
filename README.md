# **Ciheras Wind Resource Assessment**

![GitHub Header](./images/head_github.jpg)

This repository is used for documenting LBN's metmast data at Ciheras and provides introductory tutorials on analysing wind data using python via jupyter notebook.  

# **Citation**
Every usage of Lentera Bumi Nusantara's metmast data must be cited as follows:

Hilmi, F.A., Rahmatullah, U.A., 2025, _Modul Pengolahan Data_. Musthafa, A.Z.R. dan Mustopa, I.D. (editor). Ciheras: Lentera Bumi Nusantara.

This book can be downloaded through the following URL: [Modul Pengolahan Data](https://drive.google.com/file/d/19n01puDL5nDzryAnF09--Qf5VHtA5dDE/view?usp=drive_link) 

# **Metmast Details**
| Height| Installed Sensor|  Measured Quantity | Unit | Data Resolution | 
|:---:|---|:---:|:---:|:---:|
| 15 m | Vector Instruments A100R/K | Wind Speed     | m/s    | 1 s |
| 15 m | Vector Instruments W200P   | Wind Direction | degree | 1 s |
| 10 m | Vector Instruments A100R/K | Wind Speed     | m/s    | 1 s |

Notes:
- Data is retrieved from the datalogger internal storage manually. Missing data is associated to the missing retrieval. 

# **Download Data**
Data metmast (bulanan) beserta tautan unduh data dari data terbaru ke data terlama:
| Month | Data Recovery | Monthly Report | Download as parquet | Download as csv |
|---|:---:|:---:|---|---|
|2026/04 | 70,6%| [Download Report](https://drive.google.com/uc?export=download&id=1h68rJ-wt_-qIA_wDgeaje7y8Hd4r2GYs) | [LBN_2026_04.parquet](https://drive.google.com/uc?export=download&id=1FrchvYsyTS3bsPIWoUySX4hVJAoQ4eYk)| [LBN_2026_04.csv] |
|2026/03 | 39,8%| [Download Report](https://drive.google.com/uc?export=download&id=1O6KV7tW_7w10NuuZX2_Use4QYGvDTB0i) | [LBN_2026_03.parquet](https://drive.google.com/uc?export=download&id=1XqRrW3uawfypj6VQ0OjTahPdhcjSYWwR)| [LBN_2026_03.csv] |
|2026/02 | 81,5%| [Download Report](https://drive.google.com/uc?export=download&id=1PjTkEdlARoPi-DcKH53egB7w-o-o7hxb) | [LBN_2026_02.parquet](https://drive.google.com/uc?export=download&id=1NhomcQDeA8O8JUfOPwTa14qBHkispD-3)| [LBN_2026_02.csv] | 
|2026/01 | 83,2% | [Download Report] | [LBN_2026_01.parquet](https://drive.google.com/uc?export=download&id=10ApWQ4i5WtHNs-rc3AfrMI9YZRM0UtVP)| [LBN_2026_01.csv] |
|2025/12 | 13,0% | [Download Report] | [LBN_2025_12.parquet](https://drive.google.com/uc?export=download&id=1NE4T-WTIFpUx_qmLTRVgmcamEOAWgacg)| [LBN_2025_12.csv] |
|2025/11 | 97,4% | [Download Report] | [LBN_2025_11.parquet](https://drive.google.com/uc?export=download&id=1hgdUPVHP00cQQZh0QjZIpspvs4xHTYR7)| [LBN_2025_11.csv] |
|2025/10 | 44,3% | [Download Report] | [LBN_2025_10.parquet](https://drive.google.com/uc?export=download&id=1BpdS-aUdgtMz4GASrX_kWN-SuWwL2Zl6)| [LBN_2025_10.csv] |

### Python/Jupyter Notebook:
```python
import pandas as pd
url = "https://drive.google.com/uc?export=download&id=1NhomcQDeA8O8JUfOPwTa14qBHkispD-3"
df = pd.read_parquet(url)
print(df.head())
```

# **Acknowledgements**
The sensors and dataloggers in this project were supported by [ProfEC Ventus GmbH](https://www.profec-ventus.com/). 

<img src="images/ProfEC Ventus.gif" width="200">
