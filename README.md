Create or clone the repo
git clone git_link
it will pull dockerfile and other files from githhub to server

----------------Create Image----
sudo docker build . -t image_name

sudo docker images
----------------create container------------------
sudo docker run -itd -p 85:80 image_name 
sudo docker ps -a   ------list the container
-----------------get inside the container----------------------------------
sudo dockeer exec -it container_id bash
----------------------create docker image from container -----------------------------------
sudo docker commit container_id new_name


-----------------------stop/remove-----------------------
sudo docker rm -f container_id

--------------------------TAG----------------------------------
sudo docker tag image_name new_name

------------------push to dockerhub--------
sudo docker login

sudo docker push image_name:latest
