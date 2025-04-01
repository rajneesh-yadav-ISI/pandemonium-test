# EASY - Solution for the Test [GSOC-PANDEMONIUM]

## Task 1: 

### Install Pandemonium

To install **Pandemonium**, run the following command in your **R terminal**:

```r
devtools::install_github("pandemonium")
```
If you dont have package called devtools then intall it first and then try the above command

```r
install.packages("devtools")
```
## Task 2:

### Running the included example ; Finding two clustering settings that produce very different results.
```r
library(pandemonium)
pandemonium(b_anomaly$pred, b_anomaly$covInv, b_anomaly$wc, b_anomaly$exp)
```
Let the settings be as follows
**SETTING A** Linkage ="complete" ; include covarianve ="FALSE" ; Coordinates ="Pull" ; Distance measure ="euclidean" ; Number of clusters ="2" ; x = "C9" ; y = "C10"

![image](https://github.com/user-attachments/assets/fa28b65f-dea8-404e-b8ae-8c605a56fcb5)

**SETTING B** Linkage ="meadian" ; include covarianve ="FALSE" ; Coordinates ="p-val" ; Distance measure ="maximum" ; Number of clusters ="2" ; x = "C9" ; y = "C10"

![image](https://github.com/user-attachments/assets/ad701f24-73d3-4f9e-b85e-ecb557056fac)



