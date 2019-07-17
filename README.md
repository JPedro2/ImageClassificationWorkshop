## Image Classification Workshop for UK&I Co-create MeetUP | 2019

### Objectives:

1. Learn Machine Learning basics

2. Learn TensorFlow basics

3. Learn how to write an image classification model with Tensorflow

4. Learn 5 typical methods to improve model
   
### Instructions to Deploy using Google Colab:

1. Each individual model will have a [link](https://colab.research.google.com/notebooks/welcome.ipynb#recent=true) to `Google Colab`

2. Log-in to your `Google account` and make sure that you are connected to `Google Compute Engine backend`

3. Make sure that `Python3` is set and **activate** `GPU`

   *Edit > Notebook Settings > Runtime type: Python 3*
   
   *Edit > Notebook Settings > Hardware Accelerator: GPU*

4. Run each cell `sequentially` 1-by-1 **OR** Run them all at once: *Runtime > Run all* 

### Instructions to Deploy Locally:

1. Build Docker Image
``` shell
   docker build -t create_workshop .
```

2. Run Jupyter Notebook
``` shell
   docker run -it --rm -p 8888:8888 -v $(log directory on host):/tf/notebooks/logs create_workshop
```
   **visit:** http://localhost:8888
   
3. Run Tensorboard
``` shell
   docker run -it --rm -p 6006:6006 -v $(log directory on host):/tf/notebooks/logs create_workshop tensorboard --logdir=/tf/notebooks/logs
```
   **visit:** http://localhost:6006
  
