# m17n-db-rovas

## Old Hungarian (Hungarian Runes) input method for m17n-db

## What is Old Hungarian?

See:

https://en.wikipedia.org/wiki/Old_Hungarian_alphabet

http://oldhungarian.eu/index_en.html

## Mapping

See the description at the top of the hu-rovas-post.mim file.

## Dependencies

You will need to install

* ibus-m17n
* Any Unicode font supporting Old Hungarian

A font which works is available here:

https://github.com/OldHungarian/old-hungarian-font/releases

## Installation

``` bash
$ mkdir -p ~/.m17n.d/
$ cp hu-rovas-post.mim ~/.m17n.d/
$ ibus restart
```

Now ibus should list the newly added input method:

``` bash
$ ibus  list-engine | grep  -i rovas
  m17n:hu:rovas-post - rovas-post (m17n)
```

Now start ibus-setup or the Gnome3 language settings and add
the “rovas-post (m17n)” input method (Search for “Hungarian”).

