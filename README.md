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

## Adding the input method to your desktop:

### If you are  using Gnome3:

Open the regional settings in the gnome-control-center. Either from
the gnome panel by clicking on the icon showing a wrench and a
screwdriver. Then the gnome-control-center opens. Click on the flag
to go to the regional settings. You can also open the regional settings
directly by doing this on the command line:

``` bash
$ gnome-control-center region
```

In the regional settings dialog, click on the “+” button at the lower
left corner of the dialog to add an input method. In the search dialog
which opens, click on the three vertical dots at the bottom.  Enter
"rovas" into the search field. Click on “Hungarian”.  Select
“Hungarian (rovas-post (m17n))” and click on the “Add” button.

### If you are not using Gnome3:

Start ibus-setup and add the “rovas-post (m17n)” input method (Search
for “Hungarian”). Don’t use ibus-setup if you are using Gnome3, it
does not work for Gnome3!
