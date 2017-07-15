# Exploring R Markdown Websites with Stock reports

Live website is here: 

https://beta.rstudioconnect.com/content/2675/

Example code and info for R Markdown Website with Stock reports.

Requires the following packages from CRAN:

```r
install.packages(c("quantmod", "DT", rmarkdown", "flexdashboard"))
``` 

An up-to-date version of RStudio is also recommended.

R 3.2.2 used for examples.

Run the following command in the console with folder as WD with RMD files:

```
rmarkdown::render_site()
```

After running, you should see a `_Site` folder in your directory. Then open the `index.html` file in the `_site` folder and view it in your browser to see the website. If you edit and change any of the `.Rmd` files, you can use

```
rmarkdown::render_site("filename.Rmd")
```
to update the corresponding `.html` files. If you wish to add a new page to the website, create it as a `.Rmd` file, add it to appropriate place in the `_site.yml` file, and refresh the whole website using the command

```
rmarkdown::render_site()
```
