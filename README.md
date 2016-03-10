# docker-sonarr-rpi

based on https://github.com/tuxeh/docker-sonarr

## build with
docker build -t yvoswillens/sonarr:latest .

## start with 

docker run -d --restart always --name sonarr -p 8989:8989 -v /mnt/tv/:/volumes/media -v /mnt/downloads/:/volumes/completed -v /usr/local/docker/share/sonarr:/volumes/config yvoswillens/sonarr:latest -d
