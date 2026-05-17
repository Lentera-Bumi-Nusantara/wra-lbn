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
Monthly metmast data in ascending time order:
| Month | Data Recovery | Monthly Report | As parquet (raw) | As csv (raw) |
|---|:---:|:---:|---|---|
|2026/04 | 🟡70,6%| [Download Report](https://drive.google.com/uc?export=download&id=1h68rJ-wt_-qIA_wDgeaje7y8Hd4r2GYs) | [LBN_2026_04.parquet](https://drive.google.com/uc?export=download&id=1FrchvYsyTS3bsPIWoUySX4hVJAoQ4eYk)| [LBN_2026_04.csv](https://drive.google.com/uc?export=download&id=15Mi7VtfrZbKv8xY8O669P7xrBw__yTfd/view?usp=drive_link) |
|2026/03 | 🔴39,8%| [Download Report](https://drive.google.com/uc?export=download&id=1O6KV7tW_7w10NuuZX2_Use4QYGvDTB0i) | [LBN_2026_03.parquet](https://drive.google.com/uc?export=download&id=1XqRrW3uawfypj6VQ0OjTahPdhcjSYWwR)| [LBN_2026_03.csv](https://drive.google.com/uc?export=download&id=1tCqJls_Sm2CKhcB717Y7NWj2JSmTDoUC) |
|2026/02 | 🟡81,5%| [Download Report](https://drive.google.com/uc?export=download&id=1PjTkEdlARoPi-DcKH53egB7w-o-o7hxb) | [LBN_2026_02.parquet](https://drive.google.com/uc?export=download&id=1NhomcQDeA8O8JUfOPwTa14qBHkispD-3)| [LBN_2026_02.csv](https://drive.google.com/uc?export=download&id=15W4SrtC0PJe9LDK56xYGP-f2qKEZF1dm) | 
|2026/01 | 🟡83,2%| [Download Report](https://drive.google.com/uc?export=download&id=1yRmITWXB0scx6l9DsehJ62h-ydIxxVPh) | [LBN_2026_01.parquet](https://drive.google.com/uc?export=download&id=10ApWQ4i5WtHNs-rc3AfrMI9YZRM0UtVP)| [LBN_2026_01.csv](https://drive.google.com/uc?export=download&id=1EobCbwJ9Oxmq6sKsHjBPAA3WJjrPbKsI) |
|2025/12 | 🔴13,0%| Download Report | [LBN_2025_12.parquet](https://drive.google.com/uc?export=download&id=1NE4T-WTIFpUx_qmLTRVgmcamEOAWgacg)| [LBN_2025_12.csv](https://drive.google.com/uc?export=download&id=11eRnX6xLWYooW1XJWkCPpgs35_WdQl4O) |
|2025/11 | 🟢97,4% | [Download Report](https://drive.google.com/uc?export=download&id=1c1FyX6owstahf2IaamYrL9qxyG5We0tb) | [LBN_2025_11.parquet](https://drive.google.com/uc?export=download&id=1hgdUPVHP00cQQZh0QjZIpspvs4xHTYR7)| [LBN_2025_11.csv](https://drive.google.com/uc?export=download&id=1ut7NPisP-ZmN9uBDpBaKtEBQQU_5xGu9) |
|2025/10 | 🔴44,3% | [Download Report](https://drive.google.com/uc?export=download&id=11MMX-3X7CzxKC0gkTsfcSwRvceuPydFz) | [LBN_2025_10.parquet](https://drive.google.com/uc?export=download&id=1BpdS-aUdgtMz4GASrX_kWN-SuWwL2Zl6)| [LBN_2025_10.csv](https://drive.google.com/uc?export=download&id=10m5wGgYjJ3OCDyQU0WLbxF4SnOvcRkvK) |

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
