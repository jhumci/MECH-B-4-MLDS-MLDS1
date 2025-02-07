# MECH-B-4-MLDS-MLDS1 - Machine Learning and Data Science 1

Kursmaterial für eine Vorlesung eines ~1,5 * 15 Stunden (2,5 ECTS) Kurses zu grundlegenden Konzepten der Data Science. Alle Themen werden mit der entsprechenden Python-Implementierung vorgestellt. Der Kurs umfasst Grundlegendes Arbeiten mit Datenbasierter Modellierung, Grundlagen der Statistik, Lineare und nichtlineare Regression, Klassifikation, Clustering, Dimensionalitätsreduktion, und Evaluierung von Modellen.

Die Quarto Stuktur basiert auf [](https://zenodo.org/records/14697280) von [Peter Kandolf](https://orcid.org/0000-0003-3601-0852).

# Citing this project

[Citation information](CITATION.cff)


[![DOI]()]()


# Development

We use [Quarto](https://quarto.org/) to generate the lecture material.
Where we are creating a book, see [docs](https://quarto.org/docs/books/) for the structure. 
In short, each part has its own folder where you find the `qmd` files and everything is managed via `_quarto.yml`.
In order to make the use easy the entire project is managed with [pdm](https://pdm-project.org/) so to start the preview run

```bash
pdm sync
pdm quarto preview
```

The project is also compatible with the VSCode extension of Quarto, just make sure the the Python environment in `./.venv` is used. 

> [!IMPORTANT] 
> In one example `locale.setlocale(locale.LC_ALL, 'de_AT.utf8')` is used so make sure the language is installed on your system to make this example run.

# Publishing
After pushing the published website will automatically be built and deployed at [jhumci.github.io/MECH-B-4-MLDS-MLDS1/](https://jhumci.github.io/MECH-B-4-MLDS-MLDS1/).
Due to the dynamic nature of the material this might take a couple of minutes.

You can also create a pdf by calling 
```
 pdm run quarto render --to pdf
```

or the html version
```
 pdm run quarto render --to html
```

You can also find a pdf in the [releases](https://github.com/jhumci/MECH-B-4-MLDS-MLDS1/releases)