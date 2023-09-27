# places-geonames

This repository tracks the work done to identify the 600 
or so distinct place names in the LCAAJ and to sync those names with the 
GeoNames gazetteer. 

## Original Method

When compiling the LCAAJ, the researchers tagged every interviewer with a 
five-digit code that revealed their location. 
The first two digits are the latitude,
the second two digits are the longitude,
and the final digit identifies a subdivision in the bounding box where
the latitude and longitude are the southwestern corner.

As the researchers describe it,

```
     23                24
51 --|-----------------|--
     |     |     |     |
     |  7  |  8  |  9  |
     |     |   x |     |
     |-----|-----|-----|
     |     |     |     |
     |  4  |  5  |  6  |
     |     |     |     |
     |-----|-----|-----|
     |     |     |     |
     |  1  |  2  |  3  |
     |     |     |     |
50 --|-----|-----|-----|--

```

> The number of the subrectangle appears as the fifth digit of the complete
location number. The point at X in the above example is thus completely 
specified as 5023.8. The decimal point may be omitted: 50238.

Additionally, the researchers noted an “official” name for nearly every 
location and were able to solicit a “Yiddish” name from many of the
interviewees, which they recorded “in the phonological form given by the
informants, but without indication of vowel length.” The “official” name
tends to reflect upon the borders during the interwar period, meaning, 
for example, that many locations currently in Belarus or Lithuania are
listed under Polish names current in the 1930s.

Finally, the researchers split the interviewees into 11 groups with a
corresponding letter:

- A: Alsace
- C: Northern Belorus
- D: Lithuania
- G: Eastern Galicia
- H: Western Galicia
- J: Courland
- P: (Northern) Poland
- T: Transcarpathia
- V: Northern Ukraine
- W: Austria, Czechoslovakia, Germany, Holland
- X: Southern Ukraine and Rumania

## Intervening Work

Scholars using the LCAAJ have updated some of the information related to
locations, such as adding the current state in which each location can
be found or specifying the latitude and longitude more precisely than at 
the degree level. As this project continues, we will incorporate much of that
work into the data associated with the LCAAJ itself.

## Current Work in this Repository

This repository aims to harmonize the places as given in the 1961 Stabilized
Master Questionnaire with the GeoNames gazetteer, which will provide 
a unified baseline from which future place-related data analysis on the LCAAJ
can be done. The plan is to collect every hit for a populated area within
the square degree given by the place code and then editorially determine 
which response from GeoNames represents the place as listed in the 
Questionnaire and associate the GeoNames ID with the place.

Where needed, we will make interventions, and these will also be noted.

This repository is not a datastore for the places in the LCAAJ.
It is merely a record of how we built the data table.
