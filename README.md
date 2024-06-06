# pastas-data

This repository contains several datasets to serve as examples for Pastas. Each dataset is contained in an individual folder. The data itself is stored as csv-files.

## Example Usage

The datasets may be obtained through Pastas (version 1.5 or higher) using the following code:

```python
import pastas as ps

data = ps.load_dataset("collenteur_2023")  # returns a dictionary
data["heads"]  # extract the heads

```

## Datasets

The following datasets are currently available:

* `"vonk_2024"`: synthetic head data from a MODFLOW model ([Vonk et al., 2024](https://doi.org/10.5281/zenodo.10640098))
* `"collenteur_2023"`: heads and stresses from Switzerland ([Collenteur et al., 2023](https://doi.org/10.1016/j.jhydrol.2023.130120))
* `"collenteur_2021"`: timesteps of irregular ([Collenteur, 2021](https://doi.org/10.1111/gwat.13111))
* `"collenteur_2019"`: head, rain and evaporation time series from example 1 in ([Collenteur et al. 2019](https://doi.org/10.1111/gwat.12925))
* `"spek_2017"`: heads and stresses from The Netherlands ([van der Spek, 2017](https://doi.org/10.1002/2016WR019704))

See the individual subfolders for more information on each dataset.

## Notes for adding new datasets

* each dataset is contained in a folder with the name of that dataset
* each csv-file has to have a a format where the first row is the header and the first column the index of a Pandas DataFrame
* each dataset should preferably be related to a scientific publication
