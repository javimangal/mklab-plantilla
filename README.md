# Plantilla de Proyecto de R

Esta plantilla de proyectos de R ha sido modificada para contener personalizaciones mayores respecto a la [plantilla original](https://github.com/UtrechtUniversity/simple-r-project) utilizada.

## Uso 

Puedes clonar este repositorio siguiendo [estas instrucciones](https://docs.github.com/es/repositories/creating-and-managing-repositories/cloning-a-repository).  

## Project Structure

The project structure distinguishes three kinds of folders:
- read-only (RO): not edited by either code or researcher
- human-writeable (HW): edited by the researcher only.
- project-generated (PG): folders generated when running the code; these folders can be deleted or emptied and will be completely reconstituted as the project is run.

```         
.
├── .gitignore
├── CITATION.cff
├── LICENSE
├── README.md
├── preoperative_atelectasis.Rproj
├── data                  <- All project data files
│   ├── processed         <- The final, canonical data sets for modeling. (PG)
│   ├── raw               <- The original, immutable data. (RO)
│   └── temp              <- Intermediate data that has been transformed. (PG)
├── docs                  <- Documentation for users (HW)
│   ├── manuscript        <- Manuscript source, docx. (HW)
│   ├── presentations     <- Presentations, pptx, pdf. (HW)
│   ├── reports           <- Project reports, pdf. (HW)
│   └── DAG               <- Directed Acyclic Graph documentation, txt. (HG)
├── results
│   ├── output_figures    <- Figures for the manuscript or reports (PG)
│   └── output_tables     <- Output tables for the manuscript (PG)
└── R                     <- Source code for this project (HW)
    ├── scripts           <- Scripts sourced in main R markdown documents (PG)
    └── sessions          <- Text files with information of R sessions (PG)

```

## Edita el archivo de cita, licencia y gitignore

Puedes editar el archivo de cita para este repositorio [CITATION.cff](/CITATION.cff) siguiendo [estas recomendaciones](https://docs.github.com/es/repositories/managing-your-repositorys-settings-and-features/customizing-your-repository/about-citation-files).

Se ha incluido una licencia tipo MIT, que es permisiva. Si deseas conservar este tipo de licencia, recuerda cambiar tu nombre en la licencia de tu nuevo repositorio. Si deseas consultar otro tipo de licencias que se ajusten a tus necesidades, puedes [consultar esta página](https://docs.github.com/es/repositories/managing-your-repositorys-settings-and-features/customizing-your-repository/licensing-a-repository). 

El archivo [gitignore](/.gitignore) contiene instrucciones sobre los archivos que no deseas que sean rastreados ni publicados en tu repositorio de GitHub. Recomiendo usar las instrucciones default para un proyecto de R, sin embargo, puedes editar el tipo de archivos que deseas que sean visibles. 

## License

This project is licensed under the terms of the [MIT License](/LICENSE).

This project structure template repository is adapted from the [Good Enough Project](https://github.com/bvreede/good-enough-project) Cookiecutter template by Barbara Vreede (2019).
