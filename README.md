# Flask_app
Simple ML flask app to serve as template

# Make venv 
python3 -m venv ~/.Flask_ML_app
source ~/.Flask_ML_app/bin/activate

## Dir structure
```
.
├── app.py
├── data
│   └── iris_csv.csv
├── iri.pkl
├── iris.py
├── Makefile
├── model.ipynb
├── README.md
├── requirements.txt
├── static
└── templates
    ├── after.html
    └── home.html
```
    
## Functions
Makes very simple linear regression model form fixed data, saves model as pkl, runs flask app in local.

## CI
To have CI with Github actions we have the mail.yml file in .githun/workflows and the Makefil lint line.

## Docker image
Dockerfile contains docker commands to create image. 

docker build . myimage

docker run -d -p 8000:8000 --network="host" imageName

docker exec -it containerName /bin/bash


