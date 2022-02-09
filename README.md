<h1 align="center">🌌 Stellar Classification 🌌 </h1>
A classifier which classifies a set of parameters into either of Stars, Galaxies and Quasars. From Sloan Digital Sky Survey DR17

This project takes on from reading the dataset, exploring, fixing, visualizing the values, scaling the features, using different models for optimal accuracy, predicting using manually entered values, and saving the model to pickle file. The notebook is well documented and divided into steps for model making process.

The data consists of 100,000 observations of space taken by the SDSS (Sloan Digital Sky Survey). Every observation is described by 17 feature columns and 1 class column which identifies it to be either a star, galaxy or qso.

Dataset used: Stellar Classification Dataset - SDSS17

<a href="https://www.kaggle.com/fedesoriano/stellar-classification-dataset-sdss17" target="_blank">Link to the dataset</a>

### Context
In astronomy, stellar classification is the classification of stars based on their spectral characteristics. The classification scheme of galaxies, quasars, and stars is one of the most fundamental in astronomy. The early cataloguing of stars and their distribution in the sky has led to the understanding that they make up our own galaxy and, following the distinction that Andromeda was a separate galaxy to our own, numerous galaxies began to be surveyed as more powerful telescopes were built. This datasat aims to classificate stars, galaxies, and quasars based on their spectral characteristics.

### Images (Left to Right or Top to bottom)

- Quasi-stellar object
- Galaxy
- Star
<p float="left">
<img src="https://earthsky.org/upl/2019/01/quasar-artist-e1547085659933.jpg" alt="Sample Quasar Image" style="height: 150px;"/>

<img src="https://upload.wikimedia.org/wikipedia/commons/thumb/5/52/Hubble2005-01-barred-spiral-galaxy-NGC1300.jpg/1024px-Hubble2005-01-barred-spiral-galaxy-NGC1300.jpg" alt="Sample Galaxy Image" style="height: 150px;"/>

<img src="https://cdn.britannica.com/07/186507-138-CCAD17CA/Overview-types-stars-red-dwarf-giant-supergiant.jpg?w=800&h=450&c=crop" alt="Sample Star Image" style="height: 150px;"/>
</p>

### Content of data
17 feature columns and 1 class column which identifies it to be either a star, galaxy or quasar.
1. obj_ID = Object Identifier, the unique value that identifies the object in the image catalog used by the CAS
2. alpha = Right Ascension angle (at J2000 epoch)
3. delta = Declination angle (at J2000 epoch)
4. u = Ultraviolet filter in the photometric system
5. g = Green filter in the photometric system
6. r = Red filter in the photometric system
7. i = Near Infrared filter in the photometric system
8. z = Infrared filter in the photometric system
9. run_ID = Run Number used to identify the specific scan
10. rereun_ID = Rerun Number to specify how the image was processed
11. cam_col = Camera column to identify the scanline within the run
12. field_ID = Field number to identify each field
13. spec_obj_ID = Unique ID used for optical spectroscopic objects (this means that 2 different observations with the same spec_obj_ID must share the output class)
14. class = object class (galaxy, star or quasar object)
15. redshift = redshift value based on the increase in wavelength
16. plate = plate ID, identifies each plate in SDSS
17. MJD = Modified Julian Date, used to indicate when a given piece of SDSS data was taken
18. fiber_ID = fiber ID that identifies the fiber that pointed the light at the focal plane in each observation


### Models Evaluated
- Neural Network
- Random Forest Classifier
- Support Vector Machines

### Accuracy Achieved - 97.93 %
<img src="https://beeimg.com/images/q27383404472.png" alt="confusion matrix"/>


### References
https://www.kaggle.com/prasadchaskar/steller-classification-with-97-accuracy

https://www.kaggle.com/beyzanks/stellar-classification-98-4-acc-100-auc

*Project inspiration - Andy Weir's 'Project Hail Mary'*
