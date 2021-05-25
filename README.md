# Optibrium DevOps technical test

### Overview

A large part of Development Operations at Optibrium is actively developing, and supporting the development of, Python web-services.

Your solution to this problem will form the basis for the technical discussion at interview.

### Problem domain

Given an Elasticsearch index containing the following:

```json
{
    "6cafe024c7e9f79dcb654fdc34b2577a": {
        "location_on_disk": "/var/www/data/example.txt"
    },
    "cb404b5abaff0e2c302790c3d698d53a" : {
        "location_on_disk": "/var/www/data/downloads/test.txt"
    },
    "dc186f2d44cf7389606ed1da176aa854" : {
        "location_on_disk": "/var/www/data/huge_file.mp4"
    },
    ...
}
```

We would like you to develop a simple CRUD application, which will allow us to read and modify files on disk, based on the supplied document ID.

We would like you to use `Python>=3.8` and `Flask-RESTful`. We would like you to make sure your code is *fully* unit tested with `Flask-Testing`, and that there is a suitable set of BDD integration tests against elastic using `Behave`.

Finally, we would like you to provide the ability for your code to be shipped as both a source distribution, and as a *production ready* Docker image.

### Solution presentation

We would like you to create a public Git repo containing your *signed* code. In a normal setting this would then be added to a CI/CD system in order to test and build both your source distribution and your Docker image.


### Additional notes

During review we will Lint and Flake the code, and use a static analysis tool to check it against standard code quality metrics.

If you have stumbled across this tech test and want to have a go, we would love to hear from you! Please feel free to email your solution to `devops@optibrium.com`
