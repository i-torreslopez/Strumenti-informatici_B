# [Study of the nuclear activity in isolated galaxies sorted by enviroment depending on their color, morphology and star formation rate]

> [Corso di Strumenti informatici (B)]
> [Isabel Torres López]
> [Laurea Magistrale in Fisica (Astrofisica e Cosmologia)]
> [Università degli Studi di Trieste]
> [September 2026]

## In this proyect:
> Description: In this proyect I used Python to analise and treat some galaxy catalogues in order to study the effects of the Large Scale Structure on the properties of these isolated galaxies.  For my Bachelor's Thesis I studied color, morphology and star formation rate of isolated galaxies, and how Large Scale Structure (enviroment) affects these properties focusing mainly on voids and walls (given that there are not isolated galaxies in clusters according to the criteria I followed). I also studied the presence of AGN within these samples, using a catalogue I already had. For this course I wanted to deepen the study about AGN presence, so I did a comparison between isolated galaxies in voids and isolated AGN in voids, finding two really isolated ones (with distance to the nearest neighbour higher than 4MPc). I wanted to see if there was a value for tidal forces which could help me sort a galaxy in its enviroment (with dissapointing results). I also realised that in some of my catalogues there was data related to the possibility for a particular galaxy to present a barred structure, so I decided to include that as well. I then created a scripts which summarises everything I have done and creates tables for future use, in case I can continue this research at some point. 
> Contents: 
    >> Data catalogues: data used in this project, correctly quoted and referenced.
    >> Structure and scripts: thorough descriptions of each of the scripts included.
    >> Results: some plots and their descriptions.
    >> Running guide: practical instructions to ensure the correct functioning and understanding of the project.
---

## Data catalogues:

The data used in this proyect are inside the folder `data` and include:

| Data File | Content | Origin / Source |
| `SIG.txt` | catalog of SDSS-DR10 isolated galaxies| [http://cdsarc.u-strasbg.fr/viz-bin/qcat?J/A+A/578/A110#/description] |
| `Pann_SIG.csv`| [catalog of isolated galaxies in voids (some data missing)] | [Self-generated using Pan (http://www.physics.drexel.edu/~pan/) and SIG catalogs] |
| `SIG_AGN_walls.csv`| [catalog of isolated galaxies in walls with AGN presence] | [Self-generated using AGN (from https://cavity.caha.es/), Pan and SIG catalogs] |
| `Pann_SIG_ALL.csv`| [catalog of isolated galaxies in voids with all properties] | [Self-generated using AGN, Pan, Salim and SIG catalogs] |
| `SIG_Walls_ALL.csv`| [catalog of isolated galaxies in walls] | [Self-generated using AGN, Pann, Salim and SIG catalogs] |
| `sigsipsit_lss_230728_DS18.csv`| [catalog of SDSS_DR10 isolated galaxies, pairs and triplets with enviroment and morphology data] | [Self-generated using SIG catalogs and morphology data from Domínguez Sánchez (https://doi.org/10.1093/mnras/sty338)] |
| `SIG_TType.csv`| [catalog of isolated galalxies with morphology data] | [Self-generated using Domínchez Sánchez and SIG catalogs] |
| `Salim_isa.csv` | [Catalog of SDSS galaxies with explicit sSFR] |[Salim, S. 2015, arXiv preprint arXiv:1501.01963] |

---

## Structure and scripts:

The project is divided in three scripts 

*   **`250331_QLSS.ipynb`**: [Script that compares the Q_LSS (tidal force) value for every different catalogue and finds the most isolated galaxies.]
*   **`250330_Pann-SIG-AGN.ipynb`**: [Script that compares the properties of the 18 isolated AGN in voids discovered in our sample.]
*   **`250408_tables.ipynb`**: [Script that summarizes the properties of the studied galaxies in tables and studies the presence of barred galaxies in our sample.]
---

## Results

Plots and images of the results are showed within the scripts are described here:

![Result plots are stored in the folde 'plots' in png format] 
 *They show the analisis of the different properties of the isolated galaxies in voids. I have colored only the AGN for a more confortable visual, so it is easier to see which of them contain a barred structure.*

---

## Running guide:

Please follow these steps to ensure the correct running of the project:

1. Clone the repository and download the scripts
2. This project requires Python 3.10 or superior. Make sure 'matplotlib', 'numpy' and 'scipy' are correctly installed in your device.
3. Download the necessary data from this link: https://drive.google.com/drive/folders/1t_kO9dOqyZQSF9U1evTmW7uTMZJKCfdr?usp=sharing
4. Create a folder in your project branch called 'data', which should contain all the catalogues available in the link, and keep this folder in the same directory as the scripts.
5. Create a folder in your project branch called 'plots' in order for the graphics to be correctly saved in your device.
6. Run each script in the order stablished in Section 'Structure and scripts'.
7. Have a good time! :D

