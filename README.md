### This short command appends abbreviations to all of the files in a folder for example 

ASUHIC0173816_3x_shortdescription_had_lbs.jpg

UCSB-IZC00009199_had_lbs.JPG


### requires using zsh. Use this command to change shell to zsh
chsh -s /bin/zsh

### load zmv
autoload zmv

### remove n when ready to do it for real. n just prints what the command will do.
zmv -Wn '*.*' '*_had_lbs.*'

### change all names to append _dorsal_label to name
zmv -W '*.*' '*_had_lbs.*'

|Abbreviation for Image File Name|Aspect|
|had|habitus, dorsal view|
|hal |habitus, lateral view|
|hav|habitus, ventral view|
|hef|head, frontal view|
|lbs|labels|
|win|wing|
|hed|head, dorsal view|
|hef|head, frontal view|
|hev|head, ventral view|
|leg|leg|
|thd|thorax, dorsal|
|thl|thorax, lateral|
|thv|thorax, ventral|
|abd|abdomen, dorsal|
|abv|abdomen, ventral|
|abl|abdomen, lateral|
|3d|an image that is part of a 3D image|
|imt|image has typed or printed text|
|imh|image has handwritten label text|
|hab|image of habitat|
|det|image contains determination label|

### description
Free text information about the view or part. Should not use underscores in the description. Could include some code indicating different sides of a single label (a,b,c)

### 3D images
3D images have their own encoding for position based on date and time. The position needs to be recorded

```
2020-08-07-15.12.44 ZS PMax.jpg
2020-08-07-15.16.51 ZS PMax.jpg
2020-08-07-15.21.45 ZS PMax.jpg
2020-08-07-15.26.41 ZS PMax.jpg
2020-08-07-15.31.39 ZS PMax.jpg
2020-08-07-15.36.36 ZS PMax.jpg
2020-08-07-15.41.11 ZS PMax.jpg
2020-08-07-15.45.41 ZS PMax.jpg
2020-08-07-15.50.17 ZS PMax.jpg
2020-08-07-15.54.55 ZS PMax.jpg
2020-08-07-15.59.35 ZS PMax.jpg
2020-08-07-16.04.15 ZS PMax.jpg
2020-08-07-16.08.51 ZS PMax.jpg
2020-08-07-16.13.30 ZS PMax.jpg
2020-08-07-16.18.12 ZS PMax.jpg
2020-08-07-16.22.45 ZS PMax.jpg
2020-08-07-16.27.17 ZS PMax.jpg
2020-08-07-16.31.52 ZS PMax.jpg
2020-08-07-16.36.26 ZS PMax.jpg
2020-08-07-16.40.56 ZS PMax.jpg
2020-08-07-16.45.25 ZS PMax.jpg
2020-08-07-16.49.59 ZS PMax.jpg
2020-08-07-16.54.34 ZS PMax.jpg
2020-08-07-16.59.09 ZS PMax.jpg
2020-08-07-17.03.40 ZS PMax.jpg
2020-08-07-17.08.12 ZS PMax.jpg
2020-08-07-17.12.45 ZS PMax.jpg
2020-08-07-17.17.23 ZS PMax.jpg
2020-08-07-17.21.58 ZS PMax.jpg
2020-08-07-17.26.28 ZS PMax.jpg
2020-08-07-17.31.01 ZS PMax.jpg
2020-08-07-17.35.30 ZS PMax.jpg
2020-08-07-17.39.59 ZS PMax.jpg
2020-08-07-17.44.27 ZS PMax.jpg
2020-08-07-17.48.51 ZS PMax.jpg
2020-08-07-17.53.18 ZS PMax.jpg
2020-08-07-17.57.47 ZS PMax.jpg
2020-08-07-18.02.18 ZS PMax.jpg
2020-08-07-18.06.49 ZS PMax.jpg
2020-08-07-18.11.18 ZS PMax.jpg
2020-08-07-18.15.49 ZS PMax.jpg
2020-08-07-18.20.19 ZS PMax.jpg
2020-08-07-18.25.10 ZS PMax.jpg
2020-08-07-18.32.13 ZS PMax.jpg
2020-08-07-18.37.11 ZS PMax.jpg
2020-08-07-18.41.46 ZS PMax.jpg
2020-08-07-18.46.40 ZS PMax.jpg
2020-08-07-18.52.42 ZS PMax.jpg
2020-08-07-18.59.11 ZS PMax.jpg
2020-08-07-19.06.24 ZS PMax.jpg
2020-08-07-19.13.15 ZS PMax.jpg
2020-08-07-19.18.14 ZS PMax.jpg
2020-08-07-19.23.29 ZS PMax.jpg
2020-08-07-19.28.30 ZS PMax.jpg
2020-08-07-19.33.24 ZS PMax.jpg
2020-08-07-19.38.26 ZS PMax.jpg
2020-08-07-19.43.27 ZS PMax.jpg
2020-08-07-19.48.21 ZS PMax.jpg
2020-08-07-19.53.15 ZS PMax.jpg
2020-08-07-19.58.05 ZS PMax.jpg
2020-08-07-20.02.58 ZS PMax.jpg
2020-08-07-20.07.50 ZS PMax.jpg
2020-08-07-20.12.43 ZS PMax.jpg
2020-08-07-20.17.36 ZS PMax.jpg
```

