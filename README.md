### This short command appends abbreviations to all of the files in a folder for example 

ASUHIC0173816_3x_shortdescription_had_lbs.jpg

UCSB-IZC00009199_had_lbs.JPG


### requires using zsh. Use this command to change shell to zsh
chsh -s /bin/zsh

### load zmv
autoload zmv

### remove n when ready to do it for real. n just prints what the command will do.
`zmv -Wn '*.*' '*_had_lbs.*'`

### change all names to append _dorsal_label to name
zmv -W '*.*' '*_had_lbs.*'

|Abbreviation for Image File Name|Aspect|
|--------------------------------|------|
|had|habitus, dorsal view|
|hal |habitus, lateral view|
|hav|habitus, ventral view|
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

### remove whitespace and replace with underscore
`zmv -Wn '* *' '*_*'`

### 3D images
3D images have their own encoding for position based on date and time. The position needs to be recorded and kept in the file name. To update the file names:

zmv -wn '*' 'UCSB-IZC00028367_$1' #add the catalog number

zmv -Wn '* ZS PMax*' '**'

zmv -Wn '*UCSB-IZC00028367_*' '*UCSB-IZC00028367_3d_*' adds 3d code to name string

With this, the series of files below will change as shown

2020-08-07-15.12.44 ZS PMax.jpg changes to **UCSB-IZC00028367_3d_2020-08-07-15.12.44.jpg**

2020-08-07-15.16.51 ZS PMax.jpg changes to **UCSB-IZC00028367_3d_2020-08-07-15.16.51.jpg**

2020-08-07-15.21.45 ZS PMax.jpg changes to **UCSB-IZC00028367_3d_2020-08-07-15.21.45.jpg**


