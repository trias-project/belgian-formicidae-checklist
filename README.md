# Checklist of the ants in Belgium

## Rationale

This repository contains the functionality to standardize the _Checklist of the ants in Belgium_ to a [Darwin Core checklist](https://www.gbif.org/dataset-classes) that can be harvested by [GBIF](http://www.gbif.org). It was developed for the [TrIAS project](http://trias-project.be).

## Workflow

[source data](https://github.com/trias-project/belgian-formicidae-checklist/tree/main/data/raw) → Darwin Core [mapping script](https://github.com/trias-project/belgian-formicidae-checklist/blob/main/src/dwc_mapping.Rmd) → generated [Darwin Core files](https://github.com/trias-project/belgian-formicidae-checklist/tree/main/data/processed)

## Published dataset

* [Dataset on the IPT](https://ipt.inbo.be/resource?r=belgian-formicidae-checklist)
* [Dataset on GBIF](https://doi.org/10.15468/ub8mcm)

## Repo structure

The repository structure is based on [Cookiecutter Data Science](http://drivendata.github.io/cookiecutter-data-science/) and the [Checklist recipe](https://github.com/trias-project/checklist-recipe). Files and directories indicated with `GENERATED` should not be edited manually.

```
├── README.md         : Description of this repository
├── LICENSE           : Repository license
├── belgian-formicidae-checklist.Rproj : RStudio project file
├── .gitignore        : Files and directories to be ignored by git
│
├── data
│   ├── raw           : Source data, input for mapping script
│   └── processed     : Darwin Core output of mapping script GENERATED
│
└── src
    └── dwc_mapping.Rmd : Darwin Core mapping script, core functionality of this repository

```

## Installation

1. Clone this repository to your computer
2. Open the RStudio project file
3. Open the `dwc_mapping.Rmd` [R Markdown file](https://rmarkdown.rstudio.com/) in RStudio
4. Install any required packages
5. Click `Run > Run All` to generate the processed data
6. Alternatively, click `Build > Build website` to generate the processed data and build the website in `docs/`

## Contributors

[List of contributors](https://github.com/trias-project/alien-fishes-checklist/contributors)

## License

[MIT License](https://github.com/trias-project/belgian-formicidae-checklist/blob/master/LICENSE)
