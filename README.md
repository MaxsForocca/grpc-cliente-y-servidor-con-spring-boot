# gRPC Client-Server Demo con Spring Boot 3

Proyecto de una aplicación sencilla con **gRPC** usando **Spring Boot 3**, siguiendo la guía de [Dinesh Arney](https://medium.com/@dinesharney/building-a-simple-grpc-client-and-server-with-spring-boot-3-4672c1e4fab7).

## Requisitos Previos

Antes de ejecutar el proyecto, asegúrate de tener instalado:

- Java 17+
- Maven 3.8+
- IDE recomendado: VS Code
- Acceso a Internet para descarga de dependencias

## Estructura del Proyecto

El proyecto usa la estructura estándar de Maven:
```bash
grpc-cliente-y-servidor-con-spring-boot/
│
├── src/
│ ├── main/
│ │ ├── java/
│ │ └── resources/
│ └── proto/
│ └── greeter.proto <-- Definición del servicio gRPC
│
├── target/
│ └── generated-sources/ <-- Clases generadas a partir del .proto
│
├── pom.xml <-- Configuración de dependencias y plugins
└── README.md
```

## Procedimiento para ejecutar
1. Clonar el repositorio:
```bash
git clone https://github.com/MaxsForocca/grpc-cliente-y-servidor-con-spring-boot.git
cd grpc-cliente-y-servidor-con-spring-boot
```
2. Compilar el proyecto:
```bash
mvn clean package
```
3. Ejecutar:
```bash
java -jar .\target\grpc-client-server-demo-0.0.1-SNAPSHOT.jar
```
4. Probar el cliente
   En consola o una terminal:
   ```bash
   curl http://localhost:8080/greet?name=TuNombre
   ```
   En el navegador: 
   ```bash
   http://localhost:8080/greet?name=TuNombre
   ```
