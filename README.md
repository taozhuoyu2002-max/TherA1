# TherA Linux migration package

Based on https://github.com/donkeymouse/TherA . Model source: https://huggingface.co/donkeymouse/TherA . Original licenses remain applicable; see LICENSE and README.md inside the archive.

Download all five TherA-linux.zip.part files, SHA256SUMS and README-LINUX.txt from Releases into one directory.

```bash
sha256sum -c SHA256SUMS
cat TherA-linux.zip.part* > TherA-linux.zip
unzip TherA-linux.zip
```

The package includes source, required reference-cache inference weights, and the upstream testA sample. It excludes virtual environments, download caches, and personal test images. Local changes include CPU dtype compatibility, side-by-side RGB/TIR output, and output folders grouped by sampling steps. Recreate a Python environment on Linux and install CUDA-enabled PyTorch for RTX 4090. Follow README-LINUX.txt for inference.
