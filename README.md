# The Catalogue of the Rust Fungi of Belgium


## Rationale

This repository contains the functionality to standardize the _Catalogue of the Rust Fungi of Belgium_ to a [Darwin Core checklist](https://www.gbif.org/dataset-classes) that can be harvested by [GBIF](http://www.gbif.org). It was developed for the [TrIAS project](http://trias-project.be).

The Catalogue of the Rust Fungi of Belgium is a compilation of the published volumes of the "Catalogue des Uredinales de Belgique":

* Vanderweyen A & Fraiture A (2009) Catalogue des Uredinales de Belgique, 1re partie, Chaconiaceae, Coleosporiaceae, Cronartiaceae, Melampsoraceae, Phragmidiaceae, Pucciniastraceae, Raveneliaceae et Uropyxidaceae. Lejeunia, Revue de Botanique
* Vanderweyen A & Fraiture A (2009) Catalogue des Uredinales de Belgique, 2ème partie, Pucciniaceae (sauf Puccinia)(suite 2). Lejeunia, Revue de Botanique.
* Vanderweyen A & Fraiture A (2012) Catalogue des Uredinales de Belgique, 3ème partie, Pucciniaceae (genre Puccinia). Lejeunia, Revue de Botanique.

## Workflow

[source data](https://github.com/trias-project/uredinales-belgium-checklist/blob/master/data/raw) → Darwin Core [mapping script](http://trias-project.github.io/uredinales-belgium-checklist/dwc_mapping.html) → generated [Darwin Core files](https://github.com/trias-project/uredinales-belgium-checklist/blob/master/data/processed)


## Published dataset

* Dataset on the IPT(planned)
* Dataset on GBIF(planned)

## Repo structure

The repository structure is based on [Cookiecutter Data Science](http://drivendata.github.io/cookiecutter-data-science/). Files indicated with `GENERATED` should not be edited manually.

```
├── README.md         : Top-level description of the project and how to run it
├── LICENSE           : Project license
├── .gitignore        : Files and folders to be ignored by git
│
├── data
│   ├── raw           : Source data, input for mapping script
│   └── processed     : Darwin Core output of mapping script GENERATED
│
├── docs              : Repository website GENERATED
│
└── src
    ├── dwc_mapping.Rmd  : Darwin Core mapping script, core functionality of this repository
    └── src.Rproj        : RStudio project file
```

## Installation

1. Clone or fork the repository.
2. Open the RStudio project file.
3. Open the R markdown file `dwc_mapping.Rmd` in Rstudio. For more information on R markdown, click [here](https://rmarkdown.rstudio.com/)
4. Install any required packages
5. Run the code by selecting "Run All" in the "Run" menu or by using "Ctrl + Alt + R". This will generate the processed data files starting from the raw data file

## Contributors

[List of contributors](https://github.com/trias-project/uredinales-belgium-checklist/contributors)

## License

[MIT License](LICENSE)
