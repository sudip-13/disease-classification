# disease-classification
This directory peeeper disease classification
# powershell comand
# To Start docker container
docker run -it -v D:\python\deep-learning-keras\peeper-disease-classification:/peeper-disease-classification -p 8501:8501 --entrypoint /bin/bash tensorflow/serving
# To serve only latest models
tensorflow_model_server --rest_api_port=5601 --model_name=peeper-disease --model_base_path=/peeper-disease-classification/Models/
