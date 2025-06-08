# Etapa 1: compilación
FROM maven:3.9-eclipse-temurin-17 AS builder

WORKDIR /app

# Copiamos solo lo necesario primero para aprovechar la caché de dependencias
COPY pom.xml .
RUN mvn dependency:go-offline

# Ahora copiamos el resto
COPY src ./src

RUN mvn clean package -DskipTests

# Etapa 2: imagen final
FROM eclipse-temurin:17-jdk

WORKDIR /app

# Variables de entorno opcionales (pueden ser sobreescritas por docker-compose)
ENV SPRING_DATASOURCE_URL=jdbc:postgresql://localhost:5432/switcherdb
ENV SPRING_DATASOURCE_USERNAME=mouadmin
ENV SPRING_DATASOURCE_PASSWORD=220903

COPY --from=builder /app/target/*.jar app.jar

EXPOSE 8080

ENTRYPOINT ["java", "-jar", "app.jar"]
