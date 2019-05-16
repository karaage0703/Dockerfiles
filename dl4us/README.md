# dl4us
Docker image for dl4us program of Tokyo Univ. Matsuo Lab.

# Usage
Download docker image and run
```sh
$ docker run -p 8888:8888 -it --rm --name dl4us karaage0703/dl4us
```

Open new window and execute following command:
```sh
$ docker exec -it dl4us bash
```

Execute following command in container for getting dl4us program:
```sh
# cd work && git clone https://github.com/matsuolab-edu/dl4us
```

Login Jupyter Notebook on browser