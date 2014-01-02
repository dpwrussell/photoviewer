photoviewer
===========

Trivial flask application to navigate and display images.

This does nothing clever, only allows the user to navigate a file hierarchy and then display files in their original aspect ratio, but with a set width.

It would be easy to add some more advanced functionality. E.g.

[x]Render thumbnails using some image library for each image file in a listing.
[x]Thumbnails could be saved somewhere to prevent them having to be regenerated each time.
[x]A database could be added which keeps track of the thumbnails.
[x]Database could have a rating for each image.
[x]etc, etc.

Setup
-----

Install flask (http://flask.pocoo.org/)
Something like: ```pip install flask```

Clone this repository: ```git clone https://github.com/dpwrussell/photoviewer.git```

Edit photoviewer/photoviewer.py to change PHOTO_DIR to the correct place.

Symlink 'images' in static directory to PHOTO_DIR, e.g.
```
cd photoviewer/static
ln -s /Users/dpwrussell/Photos images
```

Run
---

```
cd photoviewer
python photoviewer.py
```
