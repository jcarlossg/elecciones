FROM eclipse-temurin:17
WORKDIR /app
COPY elecciones-0.0.1-SNAPSHOT.jar app.jar
COPY start.sh .
RUN chmod +x start.sh
CMD ["./start.sh"]
