# Local photo workflow

Project photos are staged locally and are not part of the repository by
default. Put every new photo in the appropriate folder inside the local inbox:

```text
photo-inbox/
```

The inbox contains folders for progress, the controller, display, each radio
module, wiring, assembly, and final-build photos. Keep the camera or phone
filename; no renaming is required. New files are reviewed for private
information, matched to the appropriate documentation section, resized if
needed, and copied into the repository only after review.

After publication, processed files can be moved to:

```text
photo-processed/
```

Photos that should not be published can be moved to:

```text
photo-hold/
```

These local folders are ignored by Git and will never be uploaded as a
directory of images.
