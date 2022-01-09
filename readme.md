# Running the notebook
To execute the analysis in the article you need an Anaconda environment with the correct packages installed. The easiest way is to simply build the docker image I used:

   docker build -t anaconda3_geo docker
   
and run the container:

   docker run --rm -it -p 8888:8888 -v $PWD:/root anaconda3_geo
   
If you want to run from scratch outside docker, the Dockerfile is a good way to go. Simply install anaconda, and use the commands I use via RUN in the docker file. 