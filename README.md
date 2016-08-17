## Build Image

`sudo docker build -t libreoffice-headless .`

## Convert office documents to pdf files

`sudo docker run  -v /YOUR_HOST_PATH/:/tmp libreoffice-headless libreoffice --headless --convert-to pdf /tmp/SOME_OFFICE_FILE --outdir /tmp`

Where YOUR_HOST_PATH is somewhere your file located in your host filesystem, and SOME_OFFICE_FILE is the office file name.

This image is based on Ubuntu 16.04 latest
