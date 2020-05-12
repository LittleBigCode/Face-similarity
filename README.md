# Face-similarity

This work is mostly inspired by : https://github.com/timesler/facenet-pytorch

The goal is to play and learn how to use a simple face similarity detection pipeline.

# Setup

1. Proceed with the installation of pytorch : https://pytorch.org/ and choose the appropiate plateforme to get the installation command.
2. Install the other requirements from the requirements.txt file using the command : pip install -r requirements.txt

# Main steps are :
1. Loading images : we use PIL lib, you may also use matplotlib insead.
2. Detect faces and cropping: using the MTCNN pre-trained model, we detect faces within the images and then crop them.
3. Compute embeddings : each image (i.e. face) will be represented by an embedding vector from facenet model
4. Similarity measure : in order to compare faces we use the euclidean distance and cosine similarity.
