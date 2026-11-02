# A Gamified LEGO Framework for Teaching Signals and Systems

This repository provides the research dataset and computational environment associated with the study **“A gamified LEGO framework for teaching signals and systems.”**

The project explores the use of hands-on LEGO-based activities and gamification to support the teaching and learning of core Signals and Systems concepts.

## Repository contents

```text
.
├── data/
│   ├── raw/
│   │   └── data_share.xlsx
│   └── processed/
├── notebooks/
│   └── gamification_analysis_zenodo.ipynb
├── environment.yml
├── LICENSE
└── README.md
```

- **`data/raw/data_share.xlsx`** — dataset shared for the study.
- **`data/processed/`** — location for derived or processed datasets, when applicable.
- **`notebooks/`** — Jupyter notebook containing the analysis workflow.
- **`environment.yml`** — Conda environment specification with the package versions used for the analyses.
- **`LICENSE`** — license governing reuse of the repository contents.

## Requirements and setup

The computational environment is managed with Conda. To create and activate it, run:

```bash
conda env create -f environment.yml
conda activate gamified-lego-signals-systems
```

Then launch JupyterLab:

```bash
jupyter lab
```

Open the analysis notebook in the `notebooks/` directory.

## Reproducibility

The `environment.yml` file specifies the versions of the Python libraries used for the statistical analyses and figures. For reproducibility, use the supplied environment rather than installing unpinned, newer package versions.

The dataset is provided in its shared form under `data/raw/`. Any data cleaning, transformations, statistical analyses, and figure-generation steps should be documented in the analysis notebook.

## Citation

If you use the dataset, code, or other materials from this repository, please cite the associated study:

> “A gamified LEGO framework for teaching signals and systems.”  
> Full publication details and the persistent DOI will be added once available.

A Zenodo record and DOI will be linked here after the repository is archived.

## License

Please refer to the [LICENSE](LICENSE) file for the terms governing the use and redistribution of the repository contents.
