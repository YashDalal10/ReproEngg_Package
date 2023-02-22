# JSON Schema Discovery project Reproducibility package

### This is a term project of Reproducibility Engineering subject Winter Semester 2022/23 offered at University of Passau.

### Short Description of the project - 

There is a growing debate about the reproduction of scientific results. Many of the published scientific results cannot be obtained again even by using the same setup. With this project, I would like to reproduce a project on JSON Schema Extraction and verify the results and claims made by the authors. The reproducibility package with all the necessary dependencies is fully automated using Docker.

The artefacts of the project are uploaded on Zenodo - 

    https://doi.org/10.5281/zenodo.7608060

The docker recipe can be downloaded from this link and then the following steps are to be used to build the project -

The most important part is to download Docker Desktop.

    docker-compose build
    
This will build the project by installing all the dependencies, cloning the original github repository of the authors and lastly the command to run the application. A mongodb image would also be created.  There are two Docker images created, 1 for mongodb database and the 2 for actual web application. The build time is approximately 2 hours on my machine. 

    docker-compose run
    
After the image is built, this command would then create a container and when the web application is opened using web browser, one can extract the JSON schema.

    docker-compose down
    
This will shut down the container.

This reproduction package is based on the project JSON Schema Discovery by Frozza, et. al. The link to their IEEE paper -

    https://ieeexplore.ieee.org/document/8424731

The link to the original code and the dependencies of the authors - 

    https://github.com/gbd-ufsc/JSONSchemaDiscovery
 
 ### Note - The mongodb to web application connection is still 'WORK IN PROGRESS!'
