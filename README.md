# Packages

sudo add-apt-repository ppa:twodopeshaggy/ppapackages

In each sub folder:

* fetch new package:

    `wget https://github.com/in0rdr/diary/archive/v0.1.tar.gz -O diary_0.1.orig.tar.gz`

* Generate data to upload, and sign it:

    `debuild  -S  -sa -k7EC3233B`

* Upload new package "changes" file:

    `dput ppa:twodopeshaggy/ppapackages diary_0.1_source.changes`
