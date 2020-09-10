# Video analysis

We examined student interactions in undergraduate physics labs using whole-class video of lab sessions. We investigated using machine learning and computer vision techniques to automatically capture student interactions. `ML-Student-Tracking` includes basic python scripts for logging positions of students and/or objects over time using *OpenCV*, an open-source computer vision library.

We used BORIS to manually code student interactions in the lab, employing two methods of video coding that separately examined student interactions within-groups or between-groups. Details of video coding and subsequent preliminary analyses and findings are described in a [paper we published in the 2020 Physics Education Research (PERC) conference proceedings](https://www.compadre.org/per/items/detail.cfm?ID=15542). The scripts and notebooks in this repository were used as part of this project and ongoing projects related to evaluation of student networks in undergraduate physics labs.

`GraphBuilder.R` includes functions for converting BORIS files into weighted adjacency matrices of student interactions, and for creating and plotting graph objects from the generated adjacency matrices. `Network_Analysis.Rmd` includes analyses that were published in the PERC conference proceedings, as well as additional unpublished analyses. `Network_Analysis-stochastic.Rmd` includes ongoing work to evaluate the evolution of networks over time. We use stochastic actor-oriented models to control for various network topology parameters and network eveolution as we examine whether/how student interactions vary with gender. We also examine how student interactions later in the semester are driven by previous interactions between individuals.