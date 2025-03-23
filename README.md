# 🎧 Sega CD Audio Extractor

**Cinepak `.S` PCM recovery tool for SEGA-CD**

🚧 **Project status: 90% – testing and refinement ongoing**  
🤝 **Contributions, feedback, and collaborations are welcome!**

This project aims to extract, reconstruct, and analyze raw PCM audio hidden in `.S` files used by SEGA-CD games, especially those that include Cinepak video sequences (e.g. *The Adventures of Batman & Robin*).

---

## 📁 Features

- Parses and extracts audio from `STAB` blocks
- Handles buffer alignment (including 256-byte hardware constraints)
- Supports stream reconstruction and block mapping
- Generates `.wav` files from raw 8-bit PCM
- Includes `.ods` spreadsheet to assist with manual block analysis

---

## 📦 Files in this repo

| File                      | Description                                                  |
|---------------------------|--------------------------------------------------------------|
| `extract_audio.py`        | Main extraction script (Python)                              |
| `cinepakfiles.ods`        | Spreadsheet to map offsets, durations and organize streams   |
| `V1.S`, `V2.S`, ...       | Sample input files from SEGA-CD game                         |
| `V1_combined_aligned.wav` | Assembled PCM WAV (aligned at 256 bytes)                     |

---

## ▶️ Usage

```bash
python3 extract_audio.py
