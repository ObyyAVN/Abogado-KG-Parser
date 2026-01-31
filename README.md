# Abogado KG Parser

Archive tools untuk **Shuumatsu no Sugoshikata ~The World is Drawing to an W/end.~** - KiriKiri Engine

## Deskripsi

Tool untuk ekstrak dan repack file archive KiriKiri (format .kg Abogado) dari visual novel berbasis Aboggado engine. 8bpp, 24bpp, 32bpp force modular injector.

## File Utama

| File | Fungsi |
|------|--------|
| `ArcKG.py` | Ekstrak file dari KG menjadi .png|
| `ArcKGPACK.py` | Pack file ke format KG |
| `ArcPACK.py` | Generic archive packer |
| `ArcPATCH.py` | Buat dan apply patch file |

## Cara Pakai

### 1. Extract Archive

```bash
python ArcKG.py archive.kg
```

File akan diekstrak ke folder `archive_extracted/`

### 2. Modifikasi File

Edit file yang sudah diekstrak sesuai kebutuhan (gambar, script, audio, dll)

### 3. Repack Archive

```bash
python ArcKGPACK.py archive_extracted/ archive_new.kg
```

### 4. Buat Patch (Optional)

```bash
python ArcPATCH.py archive_original.kg archive_new.kg patch.diff
```

## Requirements

- Python 3.x
- Modul standar Python (struct, os, sys)

