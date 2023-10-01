# Jigsaw Solver
Model to solve 6x6 Jigsaws of faces or landmarks images

## Dataset Used
- https://www.kaggle.com/competitions/mlware23/data
## Load the model using 
```sh
import pickle
pkl = open("model.pkl","rb")
model = pickle.load(open("model.pkl", "rb"))
```
## Approach
- Divided the image into 36 parts, and passed each of the part through the network ,concatenated the outputs and passed through softmax layer 
- Used Cosine Decay with restarts
- Used AdamW optimizer
## Techstack used
- Tensorflow
- Pandas
- Numpy
- Matplotlib
