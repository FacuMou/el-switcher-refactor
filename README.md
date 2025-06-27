# 🎲 El Switcher
Este proyecto es una implementación **no oficial** del juego de mesa _El Switcher_, desarrollada con fines **educativos** y como experiencia práctica en el desarrollo de aplicaciones **full-stack modernas**.

## 🚀 Tecnologías utilizadas

### 🔧 Backend (Java)
- Java 24
- Spring Boot
- Spring Web / REST API
- Spring Data JPA
- PostgreSQL
- Maven
- Docker

### 💻 Frontend (React + TypeScript)
- React
- TypeScript
- Vite
- Axios
- React Router
- Docker

### 🐳 Contenerización
- Docker
- Docker Compose

---

## 📦 Instalación y ejecución
Puedes ejecutar el proyecto de dos maneras:

### Opción 1: Con Docker (recomendado)

#### ✅ Requisitos previos
- [Docker](https://www.docker.com/) y [Docker Compose](https://docs.docker.com/compose/) instalados

#### ▶️ Pasos
1. Clona este repositorio:
```bash
git clone <repo-link>
```
2. Ejecuta la aplicación con Docker Compose:
```bash
docker-compuse up --build
```
3. Accede desde el navegador:
- Frontend: http://localhost:3000
- Backend API (Swagger UI): http://localhost:8080/swagger-ui.html

### Opción 2: Manualmente
#### Requisitos:
- [Java 24](https://www.oracle.com/java/)
- [Maven](https://www.apache.org/)
- [NodeJs](https://nodejs.org)

1. Desde la carpeta del backend ejecuta:
`mvn spring-boot:run`
Esto levanta el servidor en *http://localhost:8080*
2. Instala las dependencias con Node.js:
`npm install`
3. Ejecuta la aplicación:
`npm run dev`
Esto abrira el frontend en *http://localhost:3000*

## ⚠️ Aviso legal
Este proyecto es una implementación no oficial del juego de mesa *El Switcher* realizada con fines educativos y recreativos.
Su único propósito es servirme como práctica de programación, exploración de tecnologías back-end y front-end, y como experiencia formativa personal.
No tengo ninguna intención de monetizar, distribuir ni apropiarme de los derechos relacionados con el juego original. Todos los derechos, marcas registradas, diseños y conceptos pertenecen exclusivamente a sus respectivos creadores y/o titulares legales.
Si eres el autor o representante legal del juego y consideras que este proyecto infringe algún derecho, no dudes en contactarme y lo retiraré inmediatamente.
