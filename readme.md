# CMDev Live - Docker 101

## Ep1#

- What is docker?
- Install on windows host: https://www.youtube.com/watch?v=1G4xuqoLepI
- Install on mac host: just download and install normally
- docker hub: https://hub.docker.com/
- docker cli
  - docker ps
  - docker ps -a
  - docker pull node/mongo
  - docker images
  - docker run -it node
  - docker run -it --name my_node node
  - docker exec -it <container_id> sh
  - docker run -d --rm --name cm-mongo mongo
  - docker exec -it 1cd1d0a6bc90 sh

## Ep2#
- docker run -d --name cmdev-mongo -v /Users/../db:/data/db mongo
- docker run -d --name cmdev-mongo -v /Users/../db:/data/db -p 27019:27017 mongo