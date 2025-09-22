# Expert-Finding
The `data.csv` file contains a database collected from the open OpenAlex catalog. This database is used for expert search in the software solution.  
The program is written using the PyLucene library — a Python extension for accessing Java Lucene. To run the code, you need to install the PyLucene library.  

# Instructions for Installing PyLucene (Windows)
1) Install Docker Desktop — an application containerizer;  
2) Search for PyLucene and install the `coady/pylucene` image;  
3) Open the terminal and enter `docker run -it -p 8888:8888 coady/pylucene:latest` (for simple work with `.ipynb` later). A running container should appear in the Docker application;  
4) In VS Code, install the Docker and Dev Containers extensions, then open the running PyLucene container in a new window via the corresponding tab;  
5) Inside the container terminal, install Jupyter using `pip install jupyter`;  
6) Launch Jupyter with the command:  
   `jupyter notebook --ip 0.0.0.0 --port 8888 --no-browser --allow-root`;  
7) Open any `.ipynb` file, and in the *Select kernel* tab, paste the server link.  

# Program Explanation
- The `indexing` file performs data indexing.  
- The `testing top-k` file demonstrates the probability of an author appearing in the top-k relevant authors.  
- The `searching for quary` file performs a search among NSU researchers by query. The query itself is written in the `quary` file.  
