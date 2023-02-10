# JSON Schema Discovery project Reproducibility package

### This is a term project of Reproducibility Engineering subject Winter Semester 2022/23 offered at University of Passau.

### Short Description of the project - 

There is a growing debate about the reproduction of scientific results. Many of the published scientific results cannot be obtained again even by using the same setup. With this project, I would like to reproduce a project on JSON Schema Extraction and verify the results and claims made by the authors. The reproducibility package with all the necessary dependecnies is fully automated using Docker.

The artefacts of the project are uploaded on Zenodo - 

    https://doi.org/10.5281/zenodo.7608060

This reproduction package is based on the project JSON Schema Discovery by Frozza, et. al. The link to their IEEE paper -

    https://ieeexplore.ieee.org/document/8424731

The link to the original code and the dependencies of the authors - 

    https://github.com/gbd-ufsc/JSONSchemaDiscovery

To run the project Docker Desktop installation on local machine is required. Thats the only requirement.

After downloading the artefacts and installation of Docker, firstly the project should be built.


    The command to build is 'docker-compose build'.

    After the build is over, 'docker-compose up' starts and runs the image created.

    'docker-compose down' will stop the image.
    
 There are two Docker images created, 1 for mongodb database and the 2 for actual web application.
 
 ### Note - The mongodb to web application connection is still 'WORK IN PROGRESS!'
