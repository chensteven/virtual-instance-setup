# Virtual-instance-setup
The best virtual instance setup for data science, machine learning, deep learning and web development on Google Cloud.

## Cloud vs On-Premise Solutions
[Source](https://determined.ai/blog/cloud-v-onprem/)

## Jupyter Notebook

[Source](https://jupyter-notebook.readthedocs.io/en/latest/public_server.html)

Setting up Jupyter Notebook to be accessible through TCP port 8888
```
$ jupyter notebook --generate-config
```

```
$ jupyter notebook password
Enter password:  ****
Verify password: ****
[NotebookPasswordApp] Wrote hashed password to /Users/you/.jupyter/jupyter_notebook_config.json
```
Edit the configuration file
```
$ vi jupyter_notebook_config.py
```
Set and uncomment these fields
```
c.NotebookApp.ip = '*'
c.NotebookApp.port = 8888
```
