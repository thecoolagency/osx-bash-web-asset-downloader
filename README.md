# Web Assets Downloader for OS X

[Dependencies](#dependencies) |
[Getting started](#getting-started) |
[License](#license)

Web Assets Downloader is a script that downloads all JPG, PNG, GIF and MP4 files from the specified website site using WGET. Only to run on OS X 10.0+ (you can customize the script easily for any unix based environment).

* **WGET:** To download site files and assets
* **GREP:** To catch all lines containing the specified string (src=\"https://)
* **AWK:** To remove duplicates and filter out certain file types (js, css, pdf, mp4). You can edit the scripts to include them.
* **FIND (with XARGS):** To clean URL lines for WGET

## Dependencies

* **WGET:** To download site files and assets

Head over to [OS X Initial setup](https://github.com/thecoolagency/os-x-initial-setup) to install all required dependencies.

## Getting started

1. From your terminal run:
``` sh
wget -O - https://raw.githubusercontent.com/thecoolagency/osx-bash-web-asset-downloader/main/install.sh | bash
```
2. Then to download assets for a site run:
``` sh
sh dl-web-assets.sh
```

>:information_source: It will create a folder called domain.com in ~/Documents/web-assets and open it with Finder upon completion.

## License

Copyright (c) 2021-present Jonah L Madeya. See [LICENSE](/LICENSE.md) for further details.
