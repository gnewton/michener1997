# michener1997
LaTeX TikZ re-creation of a diagram in: 
```
    William K. Michener, James W. Brunt, John J. Helly, Thomas B. Kirchner,
    and Susan G. Stafford. 1997.
    Nongeospatial Metadata for the Ecological Sciences.
    Ecological Applications 7:1:330-342
```     
DOI: [http://dx.doi.org/10.1890/1051-0761(1997)007[0330:NMFTES]2.0.CO;2](10.1890/1051-0761(1997)007[0330:NMFTES]2.0.CO;2)


##Dependencies

* LaTeX
* TiKz
* gnuplot http://www.gnuplot.info/

##Building

###PDF

```
$ pdflatex --enable-write18 afterMichener1997page
```

###JPG
This converts the PDF file into a fairly high quality JPEG:
```
$ gs -dSAFER -dBATCH -dNOPAUSE -sDEVICE=jpeg -dDOINTERPOLATE -dTextAlphaBits=4 -dGraphicsAlphaBits=4 -r600x600 -dMaxBitmap=500000000 -dAlignToPixels=0 -dGridFitTT=2 -sOutputFile=afterMichener1997page.jpg afterMichener1997page.pdf
```

# Sample JPEG output


![alt text](https://raw.githubusercontent.com/gnewton/michener1997/master/afterMichener1997page.jpg)

