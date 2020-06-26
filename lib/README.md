## 本地非标准maven依赖库安装（解决无法传递依赖问题）

## --------------------------------------------------------------------------------install
### mvn install:install-file  -Dfile=aspose-words-jdk16-1.0.jar  -DgroupId=aspose     -DartifactId=words-jdk16  -Dversion=1.0  -Dpackaging=jar
### mvn install:install-file  -Dfile=third-jce-1.0.jar           -DgroupId=third-jce  -DartifactId=third-jce    -Dversion=1.0  -Dpackaging=jar


## --------------------------------------------------------------------------------deploy
### mvn deploy:deploy-file  -Dfile=aspose-words-jdk16-1.0.jar  -DgroupId=aspose     -DartifactId=words-jdk16  -Dversion=1.0  -Dpackaging=jar  -Durl=http://maven.aliyun.com/nexus/content/repositories/releases/  -DrepositoryId=aliyun-nexus-releases
### mvn deploy:deploy-file  -Dfile=third-jce-1.0.jar           -DgroupId=third-jce  -DartifactId=third-jce    -Dversion=1.0  -Dpackaging=jar  -Durl=http://maven.aliyun.com/nexus/content/repositories/releases/  -DrepositoryId=aliyun-nexus-releases
