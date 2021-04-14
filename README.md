## Image Classification Workshop

### Objectives:

1. Learn Machine Learning basics

2. Learn TensorFlow basics

3. Learn how to write an image classification model with Tensorflow

4. Learn 5 typical methods to improve model
   
### Instructions to deploy using [Google Colab](https://colab.research.google.com) **(recommended)**:

1. Each individual model will a `Open in Colab` button at the top that takes you to `Google Colab` and automatically loads the Jupyter notebook

2. Log-in to your `Google account` and make sure that you are connected to `Google Compute Engine backend`

3. You can use and **activate** the free `GPU`:
   
   *Edit > Notebook Settings > Hardware Accelerator: GPU*

   **Please Note:** A GPU is not required for this project, this is completely optional.

4. Run each cell `sequentially` 1-by-1 **OR** Run them all at once: *Runtime > Run all* 

5. [Click here to **START**](./model_1.ipynb)

### Instructions to deploy in your local machine (requires [docker](https://docs.docker.com/get-docker/) installed):

1. Build Docker Image
``` shell
   docker build -t create_workshop .
```

2. Run Jupyter Notebook
``` shell
   docker run -it --rm -p 8888:8888 -v $(log directory on host):/tf/notebooks/logs create_workshop
```
Grab the `notebook URL` from the output:
``` shell
[I 19:22:44.981 NotebookApp] Writing notebook server cookie secret to /root/.local/share/jupyter/runtime/notebook_cookie_secret
jupyter_http_over_ws extension initialized. Listening on /http_over_websocket
[I 19:22:45.196 NotebookApp] Serving notebooks from local directory: /tf
[I 19:22:45.196 NotebookApp] The Jupyter Notebook is running at:
[I 19:22:45.196 NotebookApp] http://dd379526f0b8:8888/?token=b38128d704f1958b585252a9132feeea81c7a95dcc48cb34
[I 19:22:45.196 NotebookApp]  or http://127.0.0.1:8888/?token=b38128d704f1958b585252a9132feeea81c7a95dcc48cb34
[I 19:22:45.196 NotebookApp] Use Control-C to stop this server and shut down all kernels (twice to skip confirmation).
[C 19:22:45.201 NotebookApp] 
    
    To access the notebook, open this file in a browser:
        file:///root/.local/share/jupyter/runtime/nbserver-1-open.html
    Or copy and paste one of these URLs:
        http://dd379526f0b8:8888/?token=b38128d704f1958b585252a9132feeea81c7a95dcc48cb34
     or http://127.0.0.1:8888/?token=b38128d704f1958b585252a9132feeea81c7a95dcc48cb34
```

   **Open the `127.0.0.1` URL to get started:** http://127.0.0.1:8888/?token=b38128d704f1958b585252a9132feeea81c7a95dcc48cb34
   
3. Click `notebooks` and start with `model_1.ipynb` and work your way through to `model_4.ipynb`
   
4. Run each cell `sequentially` 1-by-1 **OR** Run them all at once: *Cell > Run all* 