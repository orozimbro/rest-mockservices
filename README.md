# restp-mockservices
mock-services using json-server

## build and run
```
$ git clone https://github.com/orozimbro/rest-mockservices.git
$ cd rest-mockservices
$ docker rm -f rest-mocks ; docker rmi my-rest-mock:latest; docker build -t my-rest-mock .; docker run -d -p 3000:3000 -v `pwd`:/data --name rest-mocks my-rest-mock --watch db.json; docker logs -f rest-mocks
```
