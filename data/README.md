# Data Tugas 1

## Dataset yang Dipilih

Isi informasi berikut sebelum Milestone 1.

| Item | Isi |
|---|---|
| Nama dataset | `Wikipedia Indonesia (idwiki) - 20231101` |
| Sumber | `HuggingFace (wikimedia/wikipedia)` |
| Lisensi/ketentuan pakai | `CC BY-SA 4.0` |
| Ukuran | `> 500 MB, ~700.000 baris (artikel)` |
| Periode data | `Hingga November 2023` |
| Unit analisis | `Artikel Wikipedia` |

## Instruksi Unduhan Data

Anda dapat mengunduh dataset menggunakan script python yang disediakan, atau dengan menjalankan perintah berikut untuk mengunduh dataset secara manual:

```bash
python download_data.py
```
Atau menggunakan Hugging Face Datasets API untuk mendownload dan menyimpan format parquet secara langsung di folder `data/raw/`.

## Tempat Mencari Dataset

Pilih dataset Indonesia yang legal digunakan, dapat didokumentasikan sumbernya, dan memenuhi batas ukuran tugas.

| Situs | Kegunaan |
|---|---|
| [Satu Data Indonesia](https://data.go.id/) | Portal data terbuka lintas instansi pemerintah Indonesia. |
| [Badan Pusat Statistik](https://www.bps.go.id/) | Statistik sosial, ekonomi, kependudukan, dan data wilayah. |
| [BMKG Data Online](https://dataonline.bmkg.go.id/) | Data cuaca, iklim, gempa bumi, dan observasi meteorologi. |
| [Hugging Face Datasets](https://huggingface.co/datasets) | Dataset publik yang dapat dicari berdasarkan topik, bahasa, atau ukuran. |
| [Kaggle Datasets](https://www.kaggle.com/datasets) | Katalog dataset publik; periksa lisensi dan dokumentasi pembuatnya. |
| [Google Dataset Search](https://datasetsearch.research.google.com/) | Mesin pencari untuk menemukan dataset dari berbagai portal. |

## Cara Memperoleh Data

1. Buka URL sumber di atas.
2. Unduh file ke folder `data/raw/` tanpa mengubah data mentah.
3. Catat nama file dan checksum bila tersedia.
4. Ubah variabel `DATA_PATH` pada `notebooks/01_data_profiling.ipynb` agar menunjuk ke file tersebut.

## Aturan Penyimpanan

- Jangan commit dataset mentah atau hasil olahan berukuran besar ke Git.
- File pada `data/raw/` adalah data asli dan tidak boleh diubah.
- Simpan hasil transformasi yang dapat direproduksi pada `data/processed/`.
