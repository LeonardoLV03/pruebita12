# Proyecto de Microservicios

Sean todos bienvenidos a nuestro proyecto de Computacion tolerante a fallas en la cual veremos una aplicacion con microservicios la cual estara trabajando con docker y kubernetes.

## 📸 Capturas de Pantalla del Proyecto

Aquí puedes encontrar algunas capturas de pantalla que muestran la interfaz del proyecto:

1. **Home**  

![image](https://github.com/user-attachments/assets/bd91ef1b-cced-437a-abd2-6e99b471ac4a)


2. **Login**  
 
 ![image](https://github.com/user-attachments/assets/1dba0607-02cd-444b-93ff-25d2cd65eaa8)


3. **Seleccion de cuestionarios**  
 
 ![Captura de pantalla 2024-11-16 105439](https://github.com/user-attachments/assets/7ab79e51-97f3-47a2-ba68-f98425bc8a58)

4. **Cuestionarios**  
 
 ![Captura de pantalla 2024-11-16 105718](https://github.com/user-attachments/assets/02591cc6-ea8a-4134-8300-69cbe038d655)


5. **Temas de interes**  
 
 ![Captura de pantalla 2024-11-16 105831](https://github.com/user-attachments/assets/42d213c8-7260-417b-a6d7-50c5b6bf0c25)


## 📋 Descripción del Proyecto

Este proyecto esta diseñado para que los usuarios puedan responder encuestas y explorar temas de interés relacionados con la ciberseguridad. Además, integra un foro donde los usuarios pueden interactuar entre sí mediante publicaciones, fomentando el aprendizaje y la discusión sobre este tema. El sistema está desarrollado con tecnologías modernas como Docker y Kubernetes, lo que asegura una arquitectura escalable, tolerante a fallos y altamente disponible.

### Características Principales

- 📊 **Análisis de Oportunidades de Inversión**: La plataforma evalúa múltiples proyectos y presenta recomendaciones personalizadas.
- 🤖 **IA para Sugerencias**: Utilizamos GPT-3.5 y otros algoritmos para analizar los datos y sugerir las mejores oportunidades de inversión.
- 📈 **Automatización de Inversiones**: Los usuarios pueden configurar estrategias automáticas basadas en su perfil de riesgo.
- 🚀 **Despliegue en Heroku**: La plataforma se despliega fácilmente en Heroku con Docker y archivos de configuración adicionales.
- 🌐 **Modo Oscuro**: Experiencia de usuario mejorada con soporte de modo oscuro.
- 💬 **Chat de Recomendaciones con IA**: Los usuarios pueden interactuar con un chatbot que ofrece sugerencias y respuestas relacionadas con las inversiones.

## 🛠️ Tecnologías Utilizadas

- **Laravel 10**: Framework PHP para el desarrollo del backend.
- **Vue.js**: Utilizado para el desarrollo de un frontend interactivo y dinámico.
- **GPT-3.5 (ChatGPT)**: Integración con la API de OpenAI para sugerencias basadas en IA.
- **MySQL**: Base de datos relacional para almacenar datos de usuarios e inversiones.
- **Guzzle HTTP Client**: Para realizar solicitudes HTTP a la API de OpenAI.
- **Docker**: Contenedor para facilitar el despliegue.
- **Heroku**: Plataforma para el despliegue en la nube del backend.
- **mPDF**: Generación de tickets PDF para cada inversión realizada.

## 🚀 Despliegue del Proyecto

### Paso a Paso para Desplegar

Sigue los siguientes pasos para desplegar el proyecto en tu entorno local o en un servidor.

### 1. Clonar el Repositorio 🛳️

```sh
$ git clone https://github.com/tu-usuario/nuevo-proyecto-microinversiones.git
$ cd nuevo-proyecto-microinversiones
```

### 2. Configurar el Entorno 🔧

- Renombra el archivo `.env.example` a `.env`:

```sh
$ cp .env.example .env
```

- Actualiza las variables del archivo `.env` con tu configuración:
  - Configura la conexión a la base de datos (MySQL).
  - Añade las claves API para OpenAI (`OPENAI_API_KEY`).

### 3. Instalar Dependencias 🧰

Instala las dependencias de Laravel:

```sh
$ composer install
```

Instala las dependencias del frontend:

```sh
$ npm install && npm run dev
```

### 4. Generar la Clave de la Aplicación 🔑

```sh
$ php artisan key:generate
```

### 5. Migrar la Base de Datos 🗄️

Ejecuta las migraciones para crear las tablas necesarias:

```sh
$ php artisan migrate
```

### 6. Correr el Servidor Local 🚀

```sh
$ php artisan serve
```

La aplicación estará disponible en `http://localhost:8000`.

### 7. Despliegue en Heroku ☁️

- Inicia sesión en Heroku:

```sh
$ heroku login
```

- Crea una nueva aplicación en Heroku:

```sh
$ heroku create nombre-de-tu-app
```

- Añade los archivos necesarios (Procfile, Dockerfile si es necesario) y haz un push al repositorio de Heroku:

```sh
$ git add .
$ git commit -m "Despliegue en Heroku"
$ git push heroku main
```

### 8. Configurar las Variables de Entorno en Heroku 📝

Configura las variables del archivo `.env` directamente en el panel de configuración de Heroku.

## ⚙️ Uso del Proyecto

1. **Registro de Usuario**: Los usuarios pueden registrarse para crear una cuenta y acceder a la plataforma.
2. **Explorar Proyectos de Inversión**: Los usuarios podrán ver una lista de proyectos disponibles con información detallada.
3. **Recibir Recomendaciones de IA**: Basado en el perfil del usuario y las preguntas que realicen, la IA recomendará las mejores inversiones.
4. **Inversiones Automáticas**: Configura inversiones automáticas

## 📦 API Endpoints

- `POST /api/generate-text`: Utiliza la IA para responder preguntas sobre inversiones.
- `GET /api/investments`: Lista todas las oportunidades de inversión disponibles.


## 📄 Ejemplo de Archivo `.env`

```env
APP_NAME=MicroinversionesIA
APP_ENV=local
APP_KEY=base64:clave_generada_por_key_generate
APP_DEBUG=true
APP_URL=http://localhost

DB_CONNECTION=mysql
DB_HOST=127.0.0.1
DB_PORT=3306
DB_DATABASE=microinversiones
DB_USERNAME=root
DB_PASSWORD=password

OPENAI_API_KEY=tu_clave_de_openai
```

## 🔮 Futuras Mejoras

- **Soporte para múltiples idiomas** 🌍.
- **Implementación de una app móvil** 📱.
- **Sistema de notificaciones en tiempo real** 🔔.
- **Integración de más APIs para análisis financiero** 📊.

## 👥 Contribuciones

¡Las contribuciones son bienvenidas! Si quieres contribuir, por favor sigue los siguientes pasos:

1. Haz un fork del proyecto 🍴.
2. Crea una nueva rama (`git checkout -b feature/nueva-feature`) 🌱.
3. Realiza tus cambios y haz un commit (`git commit -m 'Añadir nueva feature'`) 📝.
4. Haz un push a la rama (`git push origin feature/nueva-feature`) 🚢.
5. Abre un Pull Request 🚀.

## ✨ Agradecimientos

Queremos agradecer a todas las herramientas de código abierto y a las plataformas que nos han permitido hacer realidad este proyecto. Agradecimientos especiales a:

- **Laravel** y su comunidad 🙌.
- **OpenAI** por la API de ChatGPT 🤖.
- **Heroku** por proporcionar un entorno de despliegue sencillo ☁️.

---

¡Esperamos que disfrutes usando la plataforma y que te ayude a invertir de manera más inteligente! 💡📈

Para más información, siéntete libre de contactar con nosotros o abrir un issue en el repositorio.