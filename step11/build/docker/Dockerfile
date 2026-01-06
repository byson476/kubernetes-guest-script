
FROM openjdk:17.0.2
WORKDIR /app
COPY /app/build/libs/*.jar app.jar

# 기본값(필요하면 런타임에 덮어씀)
ENV SPRING_PROFILES_ACTIVE=oracle-dev-group
EXPOSE 8080

ENTRYPOINT ["sh","-c","java -Dspring.profiles.active=${SPRING_PROFILES_ACTIVE} -jar /app/app.jar"]


