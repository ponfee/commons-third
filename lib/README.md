## 第三方jar包本地安装

- Install to local repository
```shell script
mvn install:install-file  -Dfile=aspose-words-jdk16-1.0.jar  -DgroupId=aspose     -DartifactId=words-jdk16  -Dversion=1.0  -Dpackaging=jar
mvn install:install-file  -Dfile=third-jce-1.0.jar           -DgroupId=third-jce  -DartifactId=third-jce    -Dversion=1.0  -Dpackaging=jar
```

- Deploy to remote repository
```shell script
mvn deploy:deploy-file  -Dfile=aspose-words-jdk16-1.0.jar  -DgroupId=aspose     -DartifactId=words-jdk16  -Dversion=1.0  -Dpackaging=jar  -Durl=http://maven.aliyun.com/nexus/content/repositories/releases/  -DrepositoryId=aliyun-nexus-releases
mvn deploy:deploy-file  -Dfile=third-jce-1.0.jar           -DgroupId=third-jce  -DartifactId=third-jce    -Dversion=1.0  -Dpackaging=jar  -Durl=http://maven.aliyun.com/nexus/content/repositories/releases/  -DrepositoryId=aliyun-nexus-releases
```
