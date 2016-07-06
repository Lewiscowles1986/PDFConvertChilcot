# PDFConvertChilcot
Sort of a how-to on converting PDF files to HTML

## Preparatory steps

1. Download all required PDF files
2. Place PDF files in single folder (unless you want to work in batches)
3. open a terminal and navigate to the folder (I use `~/Documents/publications/{$PUBNAME}`)

### Step 1 Convert PDF to editable ODT format

`mkdir -p ./odt && unoconv -f odt--outputpath ./odt/ *.pdf`

### Step 1b (optional) Edit ODT files, remove and replace styling as you see fit

### Step 2 Convert ODT files to HTML using Libreoffice

`mkdir -p ./html && libreoffice --headless --convert-to html --outdir ./html ./odt/*.odt`

### Improvements / Changes / Comments

Use Issues and pull-requests
