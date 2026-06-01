# 🍔🚀 Space Food

> Plataforma de e-commerce y gestión de pedidos para un restaurante temático de comida rápida espacial. 

## 📖 Sobre el Proyecto
Space Food es una aplicación web integral desarrollada como proyecto para la asignatura de **Integración de Plataformas**, durante el **4to semestre de mi carrera de Ingeniería en Informática**. Simula la operación completa de una cadena de comida rápida (estilo McDonald's, pero de temática espacial), ofreciendo tanto la interfaz de compra para clientes como paneles administrativos y operativos para el personal. El sistema destaca por la integración de múltiples servicios, incluyendo pasarelas de pago y gestión en tiempo real.

## ✨ Características Principales
* **E-commerce Completo:** Catálogo de productos ("comidas"), carrito de compras interactivo y checkout.
* **Integración de Pagos:** Conexión oficial con la API de **Mercado Pago** para procesar transacciones de forma segura, además de soporte para comprobantes de transferencia.
* **Gestión de Roles (RBAC):** Vistas y permisos personalizados con paneles dedicados para Clientes, Cocineros (`panelcocinero`) y Administradores (`panelusuarios`).
* **Control de Inventario:** APIs dedicadas para listar stock, agregar productos y un sistema automatizado de alertas para productos con stock bajo.
* **Arquitectura de API:** Endpoints RESTful construidos con Django REST Framework para el manejo asíncrono del carrito, perfiles y sucursales.

---

## 📸 Interfaz y Funcionalidades en Acción

### 1. Exploración y Menú Intergaláctico
| Menú Principal | Categoría Alienígena |
| :---: | :---: |
| <img width="400"  alt="home1" src="https://github.com/user-attachments/assets/644a35af-2e08-4aac-bbb7-6d7208670eb9" /> | <img width="400"  alt="home2" src="https://github.com/user-attachments/assets/4dd88fb4-3c71-4491-b07f-5f99564f1b33" />|
| *Página de inicio con sliders y el catálogo de comida espacial.* | *Detalle de categoría y hamburguesas temáticas.* |

### 2. Acceso y Filosofía
| Acceso de Usuarios | Quiénes Somos |
| :---: | :---: |
| <img width="400"  alt="login" src="https://github.com/user-attachments/assets/57f38382-af5e-4aa3-b0c4-174a342358f1" /> | <img width="400"  alt="somos" src="https://github.com/user-attachments/assets/e8d561e6-d9eb-4cdb-931a-0e660fc9c962" /> |
| *Portal de ingreso para clientes, cocineros y administradores.* | *Historia, misión y visión de nuestra franquicia espacial.* |

---

## 🛠️ Stack Tecnológico
* **Backend Core:** Python 3, Django 5.2, Django REST Framework
* **Base de Datos:** MySQL
* **Frontend:** Django Templates, Bootstrap 5, HTML/CSS/JavaScript
* **Integraciones y Servicios:** * Mercado Pago API (Procesamiento de pagos)
  * Firebase Admin SDK / Google Cloud (Servicios y notificaciones)
  * Ngrok (Túneles para webhooks de pago en desarrollo)

## 🚀 Instalación y Ejecución local

### Requisitos Previos
* Python 3.x
* Node.js y npm (para dependencias de Firebase/GCP)
* Servidor MySQL ejecutándose localmente

### Pasos para iniciar el entorno de desarrollo

1. **Clonar el repositorio:**
   - git clone [https://github.com/KatherinePereira/space_food.git](https://github.com/KatherinePereira/space_food.git)
   - cd space_food
2. Instalar las dependencias de Node.js:
   - npm install
3. Crear un entorno virtual de Python e instalar dependencias:
   - python -m venv venv
   - source venv/bin/activate
   - pip install django django-bootstrap5 djangorestframework mysqlclient
4. Configurar la Base de Datos:
Asegúrate de crear una base de datos en MySQL llamada pruebita y ejecuta las migraciones:
   - python manage.py makemigrations
   - python manage.py migrate
5. Configurar variables de entorno:
   - Colocar el archivo clave_spacefood.json en la carpeta config/.
   - Configurar tu MERCADOPAGO_ACCESS_TOKEN en tu archivo settings.py.
6. Ejecutar el servidor de desarrollo:
   - python manage.py runserver

## 👨‍💻 Autor
**Katherine Lisett Pereira González**
* [GitHub](https://github.com/KatherinePereira)




