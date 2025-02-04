---
title: Extras
layout: index
---


# Visual interface to activity package

Camera trap distance sampling (CTDS) is a relatively new application of distance sampling, using data from remotely-operated camera or video recorders.  The methods are described by Howe et al. (2017).  One important component of the analysis of camera trap distance sampling (CTDS) data is determining the proportion of animals that are active during the diurnal sampling window during which detections are counted.  A tool to help with this is the `activity` package (Rowcliffe et al. 2014, Rowcliffe 2021) in the `R` software.

We have created a simple interface that allows web-based access to the core functionality of the `activity` package without the need to install R.  Users can upload detection times from a text file, fit a probability density to the times, input the proportion of the day represented, and obtain activity values together with bootstrap estimates of uncertainty.  Users can download the bootstrap results file.  The activity value and bootstrap results file can then be imported into Distance for Windows for use in analysis of CTDS data.

The visual interface is built using the `shiny` package in R.  It is made available here as a free service to distance sampling users.  Please let us know if you have problems accessing it, or have suggestions for improvement.

[Click here to access the web-based interface to the activity package.](https://lenthomas.shinyapps.io/Activity/)

## References

Howe, E.J., S.T. Buckland, M.-L. Despres-Einspenner and H.S. Kuhl. 2017. Distance sampling with camera traps. Methods in Ecology and Evolution 8: 1558-1565. https://doi.org/10.1111/2041-210X.12790

Rowcliffe, M., R. Kays, B. Kranstauber, C.Carbone and P.A. Jansen. 2014. Quantifying levels of animal activity using camera trap data. Methods in Ecology and Evolution 5: 1170-1179. https://doi.org/10.1111/2041-210X.12278

Rowcliffe, M. 2021. activity: Animal Activity statistics. https://CRAN.R-project.org/package=activity



