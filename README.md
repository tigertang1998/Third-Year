# Third-Year

If R returns error when installing packages
try

```
fname <- tempfile()
download.file("https://cran.uni-muenster.de/", destfile=fname)
file.remove(fname)
```


and 

```
options(download.file.method="libcurl")
```

ref : https://stackoverflow.com/questions/33355444/r-when-trying-to-install-package-internetopenurl-failed/33372798
