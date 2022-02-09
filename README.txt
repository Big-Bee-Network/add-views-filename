This short command appends _dorsal_label to all of the files in a folder for example 
UCSB-IZC00009199.JPG is renamed to UCSB-IZC00009199_dorsal_label.JPG
UCSB-IZC00009217.JPG is renamed to UCSB-IZC00009217_dorsal_label.JPG

# requires using zsh. Use this command to change shell to zsh
chsh -s /bin/zsh

#load zmv
autoload zmv

#remove n when ready to do it for real. n just prints what the command will do.
zmv -Wn '*.*' '*_dorsal_label.*'

#change all names to append _dorsal_label to name
zmv -W '*.*' '*_dorsal_label.*'