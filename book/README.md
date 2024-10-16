# Workshop R Markdown website

This book uses R Markdown and **bookdown** (https://github.com/rstudio/bookdown).

To compile, run the following command in this directory:

```
docker run --platform linux/x86_64 -v `pwd` -it amcpherson/tidyverse:4.0.4 \
    Rscript -e "bookdown::render_book('index.Rmd', 'bookdown::gitbook')"
```

Please see the page "Get Started" at https://bookdown.org/home/about/ for more information on how to compile this book.
