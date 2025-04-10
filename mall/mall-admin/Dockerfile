# 使用官方 OpenJDK 8 镜像作为基础镜像
FROM openjdk:8-jdk-alpine

# 设置工作目录
WORKDIR /app

# 将打包后的 jar 拷贝进容器
COPY target/mall-admin-1.0-SNAPSHOT.jar app.jar

# 暴露应用端口
EXPOSE 8080

# 启动应用
ENTRYPOINT ["java", "-jar", "app.jar", "--spring.profiles.active=prod"]

