# A Gamified LEGO Framework for Teaching Signals and Systems

This repository provides the research dataset and computational materials associated with the study **“A gamified LEGO framework for teaching signals and systems.”**

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
- **`environment.yml`** — Conda environment specification, including the Python version and package dependencies.
- **`LICENSE`** — license governing reuse of the repository contents.

## Requirements and setup

The analysis environment uses Python 3.13 and Conda. From the repository root, create and activate the environment:

```bash
conda env create -f environment.yml
conda activate gamified-lego-signals-systems
jupyter lab
```

Open `notebooks/gamification_analysis_zenodo.ipynb`. If Jupyter asks for a kernel, select **Python 3 (gamified-lego-signals-systems)**.

## Running the analysis

The notebook reads the dataset from `data/raw/data_share.xlsx`. It resolves the repository root automatically when Jupyter is launched either from the repository root or from the `notebooks/` directory.

To execute the notebook from the repository root and save the cell outputs in the notebook:

```bash
jupyter nbconvert --to notebook --execute --inplace notebooks/gamification_analysis_zenodo.ipynb
```

The notebook generates publication figures in the repository-level `figures/` directory. Execution may take some time because bootstrap procedures are used.

## Reproducibility

The `environment.yml` file specifies Python 3.13 and the versions of the principal Python libraries used for the statistical analyses and figures. Use the supplied Conda environment to reduce differences caused by package-version changes.

The dataset is provided in its shared form under `data/raw/`. Data loading, derived variables, statistical analyses, and figure-generation steps are documented in the notebook. The random seed is set to `2025`; bootstrap-based procedures use 5,000 resamples.

## Citation

If you use the dataset, code, or other materials from this repository, please cite the associated study:

> “A gamified LEGO framework for teaching signals and systems.”

Full publication details and the persistent Zenodo DOI will be added here after the Zenodo record is created.

## License

Please refer to the [LICENSE](LICENSE) file for the terms governing the use and redistribution of the repository contents.
