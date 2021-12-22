# e-Book-docker
This a docker version of e-Book. For more details, you can refer to [my blog](https://www.kami-code.com/2021/12/18/SE3353-assignment10/).

## Description
You can visit the [repository]((https://github.com/Kami-code/e-Book)) for more description about APIs. The nginx is listening on port 80 and distributes the request to port 9000 and port 9001 through polling. Redis is on port 6379. MongoDB is on port 27017. MySQL is on port 3306. Neo4j is on port 7687 and 7474.(The related code is disabled for unsolved bug when using Neo4j on cluster environment.)

## Install

This project uses [docker](https://www.docker.com/) and [docker-compose](https://docs.docker.com/compose/) to run the images. Go check them out if you don't have them locally installed.

## Usage

You only need to use one command.

```
docker-compose up
```
Then you can visit the URL for details.

```
localhost:80/book/<book_id>
```

## Maintainers

~~[@Kami-code](https://github.com/Kami-code)~~

No future plan to make this docker version to keep track with the latest [e-book](https://github.com/Kami-code/e-Book) version. If you want to, you can repackage the latest e-book jar file and manually build the Dockerfile rather than using the [remote image](https://hub.docker.com/repository/docker/kamicode/e-book-docker).

## License

[MIT](LICENSE) © Kami-code