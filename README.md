**Forked with the purpose of adding the following functionality:

* Write values of data matrix to heatmap cells (done)
* Send row/column/value information to Shiny on a click/double click event (in progress)


**If you are using a version of d3heatmap older than 0.4.0, please upgrade now! Previous versions put row and column names in the incorrect order!**

___

# D3 Heatmap for R

This is an R package that implements a heatmap [htmlwidget](http://htmlwidgets.org). It has the following features:

* Highlight rows/columns by clicking axis labels
* Click and drag over colormap to zoom in (click on colormap to zoom out)
* Optional clustering and dendrograms, courtesy of `base::heatmap`

### Example

http://rpubs.com/jcheng/mtcars-heatmap

### Installation

To install:

```r
if (!require("devtools")) install.packages("devtools")
devtools::install_github("rameezsadikot/d3heatmap")
```

### Usage

Like any htmlwidget, you can visualize a d3 heatmap directly from the R console:

```r
library(d3heatmap)
d3heatmap(mtcars, scale = "column", colors = "Spectral")
```

You can also include them in R Markdown chunks, or use them in Shiny applications with the `d3heatmapOutput` and `renderD3heatmap` functions.

See `?d3heatmap` for options.
