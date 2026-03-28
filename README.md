# **Asesmen Sumber Daya Angin**

![GitHub Header](./images/head_github.jpg)

Repositori ini digunakan untuk mengelola skrip untuk pengolahan data pengukuran kecepatan angin dari tiang meteorologi di Ciheras. 

# **Sitasi**
Setiap penggunaan data metmast dari Lentera Bumi Nusantara, diharuskan menyertakan sitasi berikut:

Hilmi, F.A., Rahmatullah, U.A., 2025, _Modul Pengolahan Data_. Musthafa, A.Z.R. dan Mustopa, I.D. (editor). Ciheras: Lentera Bumi Nusantara.

Buku dapat diunduh melalui tautan berikut: [Modul Pengolahan Data](https://drive.google.com/file/d/19n01puDL5nDzryAnF09--Qf5VHtA5dDE/view?usp=drive_link) 

# **Unduh Data**
Data metmast (bulanan) beserta tautan unduh data dari data terbaru ke data terlama:
| Bulan |Data| Tautan Unduh Data|
|---|---|---|
|2026/02 | 81,5%| https://drive.google.com/uc?export=download&id=1NhomcQDeA8O8JUfOPwTa14qBHkispD-3|
|2026/01 | 83,2% | https://drive.google.com/uc?export=download&id=10ApWQ4i5WtHNs-rc3AfrMI9YZRM0UtVP|
|2025/12 | 13,0% | https://drive.google.com/uc?export=download&id=1NE4T-WTIFpUx_qmLTRVgmcamEOAWgacg|
|2025/11 | 97,4% | https://drive.google.com/uc?export=download&id=1hgdUPVHP00cQQZh0QjZIpspvs4xHTYR7|
|2025/10 | 44,3% | https://drive.google.com/uc?export=download&id=1BpdS-aUdgtMz4GASrX_kWN-SuWwL2Zl6| 

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
