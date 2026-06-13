# sal

> God Bless America

Personal portfolio and media project for Sal. This repository holds
photography, videography, creative media, personal brand assets, and
Sal Media presentation material.

Repository documentation: [docs/README.md](docs/README.md)

## Overview

This is the home base for Sal's professional creative work. It organizes
finished and in-progress media, brand assets, and client-facing
presentation material in one versioned place. Large media files are
tracked with Git LFS so the repository stays fast.

## What lives here

- Photography (edited exports, selects, retouched finals)
- Videography (edited cuts, source clips, exports)
- Creative media (design files, graphics, motion assets)
- Personal brand assets (logos, color, type, templates)
- Sal Media presentations (decks and supporting visuals)

## Project Structure

```
sal/
  README.md
  .gitignore
  .gitattributes
  photography/
    raw/            # camera originals (CR2, CR3, NEF, ARW, DNG)
    edited/         # retouched and exported finals
  video/
    source/         # source footage (MOV, MP4, MXF)
    edits/          # project files and renders
  design/           # PSD, AI, INDD and exported graphics
  brand/            # logos, palettes, type, brand guide
  presentations/    # decks and presentation media
  delivery/         # client-ready packaged output (ZIP, 7Z)
```

Adjust folders as the project grows. This is a starting layout, not a rule.

## Git LFS

Large media types are stored with Git LFS. Install and enable it once
before cloning or adding media.

```bash
# install once per machine
git lfs install

# clone with LFS support
git clone https://github.com/ssalmannyc/sal.git
cd sal
```

Tracked LFS types are defined in `.gitattributes` (PSD, AI, INDD, MOV,
MP4, MXF, WAV, TIF, TIFF, CR2, CR3, NEF, ARW, DNG, ZIP, 7Z).

Note: GitHub free accounts include limited LFS storage and bandwidth.
For large video libraries you may need a paid LFS data pack or an
external store. Official docs: https://docs.github.com/en/repositories/working-with-files/managing-large-files

## Usage

```bash
# pull latest including LFS media
git pull

# add new media (LFS handles the large files automatically)
git add .
git commit -m "Add new shoot"
git push
```

## Status

Active personal project. Structure evolves as work is added.

## License

All rights reserved. This is a personal portfolio. The media, designs,
and brand assets here are not licensed for reuse without written
permission from Sal.

## Author

Sal (https://github.com/ssalmannyc)
