# Proyecto de Microservicios

Sean todos bienvenidos a nuestro proyecto de Computacion tolerante a fallas en la cual veremos una aplicacion con microservicios la cual estara trabajando con docker y kubernetes.

## 📸 Capturas de Pantalla del Proyecto/Vista del Usuario

Aquí puedes encontrar algunas capturas de pantalla que muestran la interfaz del proyecto:

1. **Login**  

 ![Captura de pantalla 2024-11-16 110844](https://github.com/user-attachments/assets/5da63f9f-80d0-4e7b-9186-fd2a0887d316)

2. **Seleccion de cuestionarios**  
 
 ![Captura de pantalla 2024-11-16 105439](https://github.com/user-attachments/assets/7ab79e51-97f3-47a2-ba68-f98425bc8a58)

3. **Cuestionarios**  
 
 ![Captura de pantalla 2024-11-16 105718](https://github.com/user-attachments/assets/02591cc6-ea8a-4134-8300-69cbe038d655)


4. **Temas de interes**  
 
 ![Captura de pantalla 2024-11-16 105831](https://github.com/user-attachments/assets/42d213c8-7260-417b-a6d7-50c5b6bf0c25)

5. **Foro**
  
  ![Captura de pantalla 2024-11-16 110440](https://github.com/user-attachments/assets/bf6ae434-46bd-4f13-afc9-1f6eca5a1f51)

6. **Ejemplo de publicacion en el foro**
  
  ![Captura de pantalla 2024-11-16 110638](https://github.com/user-attachments/assets/b01cff33-b817-45f0-8864-27848bd5a94f)


## 📸 Capturas de Pantalla del Proyecto/Vista del Administrador

1. **Login**  

 ![Captura de pantalla 2024-11-16 110844](https://github.com/user-attachments/assets/5da63f9f-80d0-4e7b-9186-fd2a0887d316)

2. **Seleccion de cuestionarios**  
 
 ![Captura de pantalla 2024-11-16 105439](https://github.com/user-attachments/assets/7ab79e51-97f3-47a2-ba68-f98425bc8a58)

3. **Cuestionarios**  
 
 ![Captura de pantalla 2024-11-16 105718](https://github.com/user-attachments/assets/02591cc6-ea8a-4134-8300-69cbe038d655)


4. **Temas de interes**  
 
 ![Captura de pantalla 2024-11-16 105831](https://github.com/user-attachments/assets/42d213c8-7260-417b-a6d7-50c5b6bf0c25)

5. **Foro**
  
  ![Captura de pantalla 2024-11-16 110440](https://github.com/user-attachments/assets/bf6ae434-46bd-4f13-afc9-1f6eca5a1f51)

6. **Ejemplo de publicacion en el foro**
  
  ![Captura de pantalla 2024-11-16 110638](https://github.com/user-attachments/assets/b01cff33-b817-45f0-8864-27848bd5a94f)
7. **Añadir temas de interes**

  ![Captura de pantalla 2024-11-16 111117](https://github.com/user-attachments/assets/a4514b72-dc8e-4260-861b-d35e8c3a5a79)

8. **Lista de usuarios**

  ![Captura de pantalla 2024-11-16 111336](https://github.com/user-attachments/assets/6dec89d3-22e7-4fa1-8a9f-a3414a2dda0d)

9. **Actualizacion de quiz**

  ![Captura de pantalla 2024-11-16 111438](https://github.com/user-attachments/assets/31781132-d35e-4c20-b9ce-4edf66b94ec2)

10. **Ejemplo de quiz**

  ![Captura de pantalla 2024-11-16 111627](https://github.com/user-attachments/assets/44c41d8e-44e7-4714-b35b-943f7b27bc77)


## 📋 Descripción del Proyecto

Este proyecto esta diseñado para que los usuarios puedan responder encuestas y explorar temas de interés relacionados con la ciberseguridad. Además, integra un foro donde los usuarios pueden interactuar entre sí mediante publicaciones, fomentando el aprendizaje y la discusión sobre este tema. El sistema está desarrollado con tecnologías modernas como Docker y Kubernetes, lo que asegura una arquitectura escalable, tolerante a fallos y altamente disponible.

## 🛠️ Tecnologías Utilizadas

- **Express**: Framework para el desarrollo del backend.
- **React**: Utilizado para el desarrollo de un frontend.
- **Supabase**: Base de datos.
- **Docker**: Contenedor para facilitar el despliegue.

## 🚀 Despliegue del Proyecto

### Paso a Paso para Desplegar

Sigue los siguientes pasos para desplegar el proyecto en tu entorno local o en un servidor.

### 1. Clonar el Repositorio 🛳️

```sh
$ git clone https://github.com/ChristianFLozano/ProyectoSSPS.git
$ cd ProyectoSSPS
```

### 2. Instalar Dependencias 🧰
Instala las dependencias del frontend:

```sh
$ npm install && npm run dev
```
Ahora para el backend:
primero ingresa al siguiente link para encotrar el repo:  https://github.com/ChristianFLozano/ProyectoSSPSBackend

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