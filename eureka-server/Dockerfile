FROM openjdk:17-jdk-slim

VOLUME /tmp
COPY target/*.jar app.jar
EXPOSE 8761

# 设置JVM参数
ENV JAVA_OPTS="-Xmx512m -Xms256m"



# 使用shell格式的ENTRYPOINT，这样可以使用环境变量
ENTRYPOINT java $JAVA_OPTS -jar /app.jar