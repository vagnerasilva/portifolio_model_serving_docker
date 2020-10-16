

https://neptune.ai/blog/how-to-serve-machine-learning-models-with-tensorflow-serving-and-docker?utm_source=facebook&utm_medium=post-in-group&utm_campaign=blog-how-to-serve-machine-learning-models-with-tensorflow-serving-and-docker&utm_content=BigDataPakistan&fbclid=IwAR0EEu9sA4x1hfsJjqS1aM_WjCcRG9VSCingGLs-dyEuE_0ieO3Oiq997yw




## Modelo tensorflow em docker

# Parte 1
docker pull tensorflow/serving

# part2 executando docker
docker run -p 8501:8501 --name tfserving_classifier --mount type=bind, source=./img_classifier/,target=/models/img_classifier -e MODEL_NAME=img_classifier -t tensorflow/serving


 docker run -p 8501:8501 --name tfserving_classifier \
 --mount type=bind,source=/Users/nameuser/Desktop/deepIA/dockerML/img_classifier/,target=/models/img_classifier \
 -e MODEL_NAME=img_classifier -t tensorflow/serving


virtualenv -p python3 .

 source ./bin/activate


 TODO: Evoluir para docker-compose