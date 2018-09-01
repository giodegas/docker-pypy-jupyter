# docker-pypy-jupyter
[Jupyter Notebook](http://jupyter.org) running with a [PyPy](http://pypy.org) accelerated Python3 kernel

1. pull the image:

``docker pull giodegas/pypy-jupyter``

2. create and run the container instance:

``docker run -it -p 8888:8888 --name jup giodegas/pypy-jupyter /bin/bash``

3. launch jupyter notebook server inside the container:

``jupyter notebook --allow-root --ip=0.0.0.0 --no-browser``

4. you should get something like, where you have to pick the token which changes everytime:

```
[I 10:13:28.926 NotebookApp] Serving notebooks from local directory: /
[I 10:13:28.926 NotebookApp] The Jupyter Notebook is running at:
[I 10:13:28.926 NotebookApp] http://(28a6a4bf5fd3 or 127.0.0.1):8888/?token=b20247c869adb06c7ff7ec2e9c97b260681e5a5080777fa7
[I 10:13:28.927 NotebookApp] Use Control-C to stop this server and shut down all kernels (twice to skip confirmation).
[C 10:13:28.928 NotebookApp]

    Copy/paste this URL into your browser when you connect for the first time,
    to login with a token:
        http://(28a6a4bf5fd3 or 127.0.0.1):8888/?token=b20247c869adb06c7ff7ec2e9c97b260681e5a5080777fa7
```

5. then launch in your browser the URL with the right token:

```http://127.0.0.1:8888/?token=b20247c869adb06c7ff7ec2e9c97b260681e5a5080777fa7```
