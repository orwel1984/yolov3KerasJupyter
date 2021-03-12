# yolov3KerasJupyter
A Jupyter notebook with implementation of pre-trained Yolo-v3 in Keras.


### Step 1: Clone the repository & cd to working directory
1. git clone https://github.com/orwel1984/yolov3KerasJupyter.git
2. cd yolov3KerasJupyter

### Step 2: Build the Docker container to Run the Notebook server
docker build . -t orwel84/notebooks:gpu-py3-jupyter-opencv

### Step 3: Run the container
docker run -it --rm -v $(realpath yolov3KerasJupyter):/tf -p 8888:8888 -p 443:443 --gpus all orwel84/notebooks:gpu-py3-jupyter-opencv

### Step 4: Open the notebook
1. Follow the commandline instrunctions from Step-3 and open the notebook url in the browser. 
2. Open the notebook file "Yolo-v3 Object Detection using Keras".ipynb

