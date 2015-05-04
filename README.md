# docker-sbt
Put SBT into a Docker container.

## Usage
Run SBT container with local SBT directories mounted

```sh
docker run -it -v $HOME/.sbt:/sbt -v $HOME/.ivy2:/ivy2 -v $PWD:/project jehrhardt/sbt
```
