FROM java:8

MAINTAINER Jan Ehrhardt <jan.ehrhardt@gmail.com>

ADD https://repo.typesafe.com/typesafe/ivy-releases/org.scala-sbt/sbt-launch/0.13.8/sbt-launch.jar /opt/sbt-launch.jar

WORKDIR /project

ENTRYPOINT ["java", "-Xms512M", "-Xmx1536M", "-Xss1M", "-XX:+CMSClassUnloadingEnabled", "-Dsbt.global.base=/sbt/0.13", "-Dsbt.ivy.home=/ivy2", "-Dsbt.boot.directory=/sbt/boot", "-jar", "/opt/sbt-launch.jar"]
