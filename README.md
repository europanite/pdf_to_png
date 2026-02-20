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
