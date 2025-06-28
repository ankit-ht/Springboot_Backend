FROM openjdk:17-jdk-slim

# Install Maven
RUN apt-get update && apt-get install -y maven && rm -rf /var/lib/apt/lists/*

WORKDIR /app

# Copy the full project (not just the JAR)
COPY . .

EXPOSE 8087

ENTRYPOINT ["mvn", "spring-boot:run"]
