# bm-kailath-linear-systems
## DjVu bookmark for Kailath's Linear Systems 
You know where to find the book. I suggest you use the .djvu version that has 704 pages.

.pdf version is of poor quality and I am not hopeful with any OCR results.

Thus using the .djvu version makes sense. Since the book is relatively long and depends heavily on references on different chapters, I thought that a bookmark would be useful for the reader. Thus spent couple hours to write it since I constantly check the book for reference.

You will need DjVuLibre. On Windows you need to add the install path to your environmental variable and to your `%PATH%` unless you want cmd.exe 10 line command cancer.
```
 djvused kailath.djvu -e "set-outline kailath.bm" -s
```
I converted my .djvu version to .pdf via https://oracleyue.github.io/post/djvu2pdf_with_toc/ which transfers the .djvu bookmarks to the .pdf
`pdftk` and 'sexpdata' library needed.

If you have the .pdf version, you can just use:
```
pdftk kailath.pdf update_info "kailath-metadata.in" output kailath-w-bm.pdf
```
Please disseminate. If you find any errors/typos please report.
