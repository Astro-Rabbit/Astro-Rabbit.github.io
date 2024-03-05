+++

template = "post.html"
title = "Spectroscopic Distance, Mass, and Age Estimations for APOGEE DR17"
date = 2024-02-01

[extra]
abstract = "We derive distances and masses of stars from the Sloan Digital Sky Survey (SDSS) Apache Point Observatory Galactic Evolution Experiment Data Release 17 using simple neural networks. Training data for distances comes from Gaia EDR3, supplemented by literature distances for star clusters. For masses, the network is trained using asteroseismic masses for evolved stars and isochrone masses for main-sequence stars. The models are trained on effective temperature, surface gravity, metallicity, and carbon and nitrogen abundances. We found that our distance predictions have median fractional errors that range from ≈20% at low log g and ≈10% at higher log g with a standard deviation of ≈11%. The mass predictions have a standard deviation of ±12%. Using the masses, we derive ages for evolved stars based on the correspondence between mass and age for giant stars given by isochrones. The results are compiled into a Value Added Catalog called DistMass that contains distances and masses for 733,901 independent spectra, plus ages for 396,548 evolved stars."

authors = ["Alexander Stone-Martinez, Jon Holtzman, + 4 others"]

links = [
    { name = "ADS", link = "https://ui.adsabs.harvard.edu/abs/2024AJ....167...73S/abstract" },

]

publication = "ApJ" 
year = 2024

image = { path = "DistMassResults.jpg", style="figure", caption = "C/N–mass relation for the ML model predictions trained on all six seismologies/corrections. Color coded by Fe/H and binned in log g intervals of 0.5." }

+++

