# Beego Framework

An open source framework to build and develop your applications in the Go way

More info: https://beego.me/

# [Install Beego](https://beego.me/quickstart)

The bee cli is a tool to initialize, develop, scaffold and maintain the Go applicacation.
To install or upgrade Beego and the Bee dev tool:

    go get -u github.com/astaxie/beego
    go get -u github.com/beego/bee

# Useful commands

### Run project

The bee run command will supervise the file system of any Beego project using inotify. The results will autocompile and display immediately after any modification in the Beego project folders.

Navigate to the service project: 'fismobile.com/mb-config-tool/service'.

    bee run

Visit http://localhost:9000/

### Pack project
The pack command is used to compress the project into a single file. The compressed file can be deployed by uploading and extracting the zip file to the server.

    bee pack

### Build and run with Docker

NOT COMPLETED

    bee dockerize -image="library/golang:1.6.4" -expose=9000
    bee help dockerize


### [Swagger](https://beego.me/blog/beego_api)
To go to swagger doc visit:
    
    /swagger


to generate the new doc run:
    
    bee run -downdoc=true -gendoc=true


### [Code generator](https://beego.me/docs/install/bee.md#command-generate)

This command will generate the routers by analyzing the functions in controllers.
It works similar to "ng generate <>" from angular.

    bee generate model [modelname] [-fields=""]
        generate RESTful model based on fields
        -fields: a list of table fields. Format: field:type, ...
    
    bee generate controller [controllerfile]
            generate RESTful controllers
    
    bee generate test [routerfile]
        generate testcase





### My Examples:
- TBD
