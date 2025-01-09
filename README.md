# big-data-platforms

University of Helsinki [Big Data Platforms](https://big-data-platforms-24.mooc.fi/) course assignments. The assignments are done in Jupyter Notebook. You can run them on any platform, VS Code also has extensions for it.

## Instructions for Docker

Instructions copied from course details.

Make sure you have Docker installed.

Pull the Jupyter Notebook image:

```
docker pull hainingt/big_data_platforms:2024
```

Start a Jupyter Notebook container:

```
docker run --name bdp_homework --rm -p 8888:8888 -v
.:/home/jovyan/work hainingt/big_data_platforms:2024
```

Some notes about the above command:
In case of you cannot find the local folder in the Jupyter Notebook, please check the permission of
the folder. You can change the permission by running the following command before starting the
container:

```
chmod 777 -R .
```

Open the jupyter notebook in your browser by copying the URL with the token from the terminal or
command prompt. The URL should look like this:

```
http://127.0.0.1:8888/?token=<TOKEN_VALUE>
```