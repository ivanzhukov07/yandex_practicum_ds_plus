# Russian film distribution research

## Description of the project

The customer of this research is the Ministry of Culture of the Russian Federation.
You need to study the Russian film distribution market and identify current trends. Pay attention to films that have received government support. Try to answer the question of how interesting such films are to the viewer.
You will work with data published on the open data portal of the Ministry of Culture. The data set contains information about distribution certificates, box office and government support for films, as well as information from the KinoPoisk website.

## Description of data

The `mkrf_movies` table contains information from the rental license registry. One film can have several distribution certificates.
- `title` - the title of the movie
- `puNumber` - rental certificate number
- `show_start_date` - movie premiere date
- `type `- movie type
- `film_studio` - production studio
- `production_country` - country of origin
- `director` - director
- `producer` - producer
- `age_restriction` - age category
- `refundable_support` — amount of state support refundable funds
- `nonrefundable_support` - the amount of non-refundable state support funds
- `financing_source` - source of government funding
- `budget` - the total budget of the movie
- `ratings` - movie rating on KinoPoisk
- `genres` - the genre of the movie

Note that the budget column already includes full government support. The data in this column is only for those films that received government support.

The `mkrf_shows` table contains information about movie screenings in Russian cinemas.
- `puNumber` - rental certificate number
- `box_office` - fees in rubles

## Tools used

`pandas` `numpy` `matplotlib` `math`
