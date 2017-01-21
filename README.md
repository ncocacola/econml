# EconML

## Python
```
git clone https://github.com/ncocacola/econml
pip install -r requirements.txt
jupyter notebook
```

## R
For the `R` Kernel to work in Jupyter, you will need to run the following commands from Terminal assuming you already have `R` installed):
```
R -e "install.packages(c('repr', 'IRdisplay', 'evaluate', 'crayon', 'pbdZMQ', 'devtools', 'uuid', 'digest'), repos='https://cran.ma.imperial.ac.uk/')"
R -e "devtools::install_github('IRkernel/IRkernel')"
R -e "IRkernel::installspec()"
```

You will also need to install the following packages, specifically for the experiments we run:

```
R -e "install.packages(c('RSQLite'), repos='https://cran.ma.imperial.ac.uk/')"
```
