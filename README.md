# real-time-feature-extraction-and-image-segmentation-
real time feature extraction and image segmentation using remote sensing and deep learning
![image](gifs/image2.gif)

## Installation:
* Simply run the command ***pip install -r requirements.txt*** to install the necessary dependencies.
* In case you need to use your GPU for computation, ensure that you have the right CUDA drivers and CUDNN installed.

## Usage:
1. Simply run the command: 
```
streamlit run app.py
```
2. Navigate to http://localhost:8501 in your web-browser.
3. By default, streamlit allows us to upload files of **max. 200MB**. If you want to have more size for uploading audio files, execute the command :
```
streamlit run app.py --server.maxUploadSize=1028
```

# Videos
| **Original Video**  | **Segmented Video**  |
|---------------------|-----------------------|
| ![pic1](gifs/1.gif)  | ![pic1](gifs/segmented_1.gif)  |


### Running the Dockerized App
1. Ensure you have Docker Installed and Setup in your OS (Windows/Mac/Linux). For detailed Instructions, please refer [this.](https://docs.docker.com/engine/install/)
2. Navigate to the folder where you have cloned this repository ( where the ***Dockerfile*** is present ).
3. Build the Docker Image (don't forget the dot!! :smile: ): 
```
docker build -f Dockerfile -t app:latest .
```
4. Run the docker:
```
docker run -p 8501:8501 app:latest
```

This will launch the dockerized app. Navigate to ***http://localhost:8501/*** in your browser to have a look at your application. You can check the status of your all available running dockers by:
```
docker ps
```
