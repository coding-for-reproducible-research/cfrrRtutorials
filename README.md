# cfrr-r-tutorials

This GitHub Repository contains the source code for an R package that is used to distribute R tutorials developed by the Coding for Reproducible Research Programme at the University of Exeter. These tutorials have been developed with the learnr package.


## Installation

Below we provide complete instructions on how to install the necessary dependency packages and open the tutorials. 

First we need to (install and) load two packages from CRAN to ensure R has the required functions. This can be done with the following code:

```
install.packages("devtools") 
install.packages("learnr") 
library(devtools)
library(learnr)

```

With these successfully installed we can now install the package from this repository.

```
devtools::install_github("coding-for-reproducible-research/cfrrRtutorials")
```

This package includes a number of tutorials that we deliver workshops on. Each tutorial comes in an interactive document with the course notes, code examples, exercises and quiz questions. Therefore these also function as self contained study notes which you can work through at your pace. 

To get a list of the tutorials we currently have available you can run

```
available_tutorials("cfrrRtutorials")
```

This should give a list like the following

```
Available tutorials:
* cfrrRtutorials
  - Introduction to Regression with R                       : "Introduction to Regression with R"
  - Mixed Effects Regression with R                         : "Mixed Effects Regression with R"
  - Regression Analysis in R: Adapting to Varied Data Types : "Regression Analysis in R: Adapting to Varied Data Types" 
```


You can launch any of these tutorials with the `run_tutorial` function from the `learnr` package. Note, upon execution the command below first needs to build the interactive elements. This may take a few minutes.  The progress of the build can be seen in the **Jobs** tab in the bottom left panel of Rstudio.

For example to launch the "Introduction to Regression with R " tutorial which is an introductory course , you can run:

```
learnr::run_tutorial("Introduction to Regression with R", "cfrrRtutorials")
```

When ready the tutorial may launch in a new window, or (more likely) there will be some output in red in the **Jobs** console that says something like:  

```
Output created: Introduction-to-Regression-with-R .html

Listening on http://127.0.0.1:38555

+------------------------------------------------------------------------+
<U+2713> Open the tutorial in your browser: http://127.0.0.1:38555
! Stop or cancel this job to stop running the tutorial
+------------------------------------------------------------------------+
```

If the tutorial does not automatically launch in a new window, to launch it copy the web address in this case (http://127.0.0.1:38555) into a web browser of your choice, such as Chrome. 

You can then start the workshop in this document. You can navigate through the sections using the menu on the side. Please note that the data required for the examples and exercises is pre-loaded within each interactive document, so the commands/exercises only work within it. They won't work with the Rstudio console. When you come to apply what you have learned on your own datasets, you will need to ensure your data is loaded and edit the syntax to model the relevant variables. 

# Contact details

Please contact CodingForReproducibleResearch@exeter.ac.uk for details on these workshops.

# Contributions guidelines

Contributions to this repository follow those set out by the wider Coding For Reproducible Research Programme. Details can be found here:<insert link>.

# Acknowledgements

These materials were developed by Eilis Hannon and Conor Crilly as part of the Coding For Reproducible Research Programme. 
