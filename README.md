# Packages

In each sub folder:

* fetch new package:

    `wget https://github.com/xxx/xxx/archive/v2.8.tar.gz -O xxx_2.8.orig.tar.gz`

* Generate data to upload, and sign it:

    `debuild  -S  -sa -k7EC3233B`

* Upload new package "changes" file:

    `dput ppa:twodopeshaggy/xxx xxx_2.8_source.changes`
