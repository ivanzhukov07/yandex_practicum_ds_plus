# Determining star temperature

## Description of the project

We received a task from the observatory: to figure out how to use a neural network to determine the temperature on the surface of detected stars. 

Usually , scientists use the following methods to calculate the temperature:

- The law of displacement of Wine
- Stefan-Boltzmann Law
- Spectral analysis

Each of them has pros and cons. 

The observatory wants to introduce machine learning technologies to predict the temperature of stars, hoping that this method will be the most accurate and convenient.

The observatory's database contains the characteristics of 240 stars that have already been studied.

## Description of data

**Features**

- Relative luminosity **`L/Lo`** — luminosity of a star relative to the Sun
- Relative radius **`R/Ro`** — radius of the star relative to the radius of the Sun
- Absolute magnitude **`Mv`** — a physical quantity that characterizes the brilliance of a star
- Star color (**`white`**, **`red`**, **`blue`**, **`yellow`**, **`yellow-orange`**, etc.) — the color of the star, which is determined on the basis of pectral analysis
- Type of star

| Type of star | The number corresponding to the type |
| ------|------ |
| Brown dwarf | 0 |
| Red Dwarf | 1 |
| White dwarf | 2 |
| Main sequence stars | 3 |
| Supergiant | 4 |
| Hypergiant | 5 |

- Absolute temperature **`T(K)`** — temperature on the surface of the star in Kelvins.


## Tools used

`sklearn` `scipy` `matplotlib` `pandas` `numpy` `pytorch`

## Models used

`neural network`

## Addition tools

`OneHotEncoder` `StandardScaler` `dropout_optimization` `batch_size_optimization`

## Metrics

`mean_squared_error`
