This project contains Apache Spark experiments I implemented as part of learning Spark.

These experiments are based on:

* Python 3.5
* Apache Spark 2.X
* pyspark
* IPython / Jupyter

The experiments are in the form of Jupyter notebooks that may be executed.

# Installation

You'll need the above dependencies to run the notebooks.  You can install the dependencies yourself, but if you don't already have them set up, an easier way to go is to use this ready-made Docker image:

* https://github.com/jupyter/docker-stacks/tree/master/pyspark-notebook

To install and run:

1. Install Docker: https://docs.docker.com/engine/installation/
2. Create and run a Docker container based on the above pyspark-notebook image:

  ```
  > export SPARK_EXPERIMENTS=<full path to directory containing this project>
  > docker run -d -p 8888:8888 -v $SPARK_EXPERIMENTS:/home/jovyan/work --name spark-experiments jupyter/pyspark-notebook
  ```

3. Open http://127.0.0.1:8888
4. If the above URL doesn't work, use the IP address of the Docker machine:
```
> docker-machine ip <name of your running Docker machine>   # See 'docker-machine ls' if you don't know the name
```

# Exported notebooks

Following are HTML exports of the notebooks:

* [basic_experiments](https://rawgit.com/rsmith72/spark-experiments/master/basic_experiments.html)

