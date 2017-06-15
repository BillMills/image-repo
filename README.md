# image-repo

A demonstration repo for a version-controlled collection of images browsable by tag.

## Quickstart

```
git clone https://github.com/BillMills/image-repo
cd image-repo
docker container run -v $(pwd):/app/static/image-repo -p 8080:5000 -d billmills/whalepic:0.1
```

Visit `127.0.0.1:8080` in your browser (Chrome recommended), and click on some tags on the left to see a selection of corresponding figures.

## Image repo format

 - Each image or group of related images goes in its own directory
 - Each such directory contains a file `tags`; this file lists the tags associated with this image, one per line.