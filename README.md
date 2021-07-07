# docker-spark

This tutorial will help you set up the Docker with simulated HDFS and Spark cluster with 1 Spark master and 3 Spark workers, then run a simple MapReduce job. 


1. Download and install Docker from https://docs.docker.com/get-docker/


2. Clone this git repo


3. Open Bash/Terminal at the folder location (For Windows, please use Git Bash)

If you don't have Git Bash, download and install here: https://git-scm.com/downloads


4. Build Docker images using command:

```
./build.sh
```

You might need to change mode to make the file executable by running the command:
```
chmod 777 build.sh
```

More about chmod here: https://en.wikipedia.org/wiki/Chmod


5. Compose the containers by running the command:

```
docker-compose up
```

Congratulations! You got your Docker environment set up. Now you can access the Spark Master UI at port 8080, Jupyter Lab at port 8888 and Spark Worker UI at port 8081 and 8082 accordingly.


6. Upload jupyter notebook to Jupyter Lab and test run the simple map reduce job for pi estimation.

What if I want to have 3 workers instead? Where and how should I update my setup files to do this? Is there any difference between 2 workers and 3 workers cluster for this map reduce job? Hint: check the other docker-compose file.


7. Now test the same notebook on Databricks:

Log in to Databricks Community: https://community.cloud.databricks.com/login.html

Create a test cluster, upload the notebooks and test run it.


8. Let's try to run a SparkML notebook imported from this link on Databricks https://docs.databricks.com/_static/notebooks/getting-started/get-started-with-mllib-dbr7.html 