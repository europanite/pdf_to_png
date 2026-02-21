# [PDF to PNG](https://github.com/europanite/pdf_to_png "PDF to PNG")

[![License](https://img.shields.io/badge/License-Apache_2.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
![OS](https://img.shields.io/badge/OS-Linux%20%7C%20macOS%20%7C%20Windows-blue)

# pdf_to_png
Snipets to translate pdf files to png files.

# Usage
```bash
sudo apt update
sudo apt install poppler-utils -y
mkdir -P png
for fn in `ls  ./pdf/*.pdf | xargs -i basename {}`;
    do pdftoppm -png  pdf/$fn png/${fn%.pdf}.png;
done

```
