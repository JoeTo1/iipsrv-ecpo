1. create a physical directory on your disk:
c://data/images/imageStorage/ecpo_new/

2. upload image2.tif into the folder

3. Start Docker image and port (windows enviroment)

docker run -d -p 8000:80 JoeTo1/iipsrv-ecpo
docker run -d -p 8000:80 -v c:/data:/data JoeTo1/iipsrv-ecpo

4. Open Browser and open image on iip-webserver

-> http://localhost:8000/cgi-bin/fcgi-bin/iipsrv.fcgi?IIIF=imageStorage%2Fecpo_new%2Fimage2.tif%2Ffull%2F!648,390/0/default.jpg

image-server is working!

5. copy iifjpgdocktest.php and iifjpgdock.php on your local-webserver
6. open http://localhost/iifjpgdocktest.php on your local-webserver

