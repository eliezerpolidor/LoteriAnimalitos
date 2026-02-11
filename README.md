🚀 Sistema de Gestión de Loterías y Apuestas (Animalitos)
Este proyecto tiene como objetivo desarrollar un sistema integral para la gestión de apuestas de loterías de "Animalitos", ofreciendo una plataforma robusta y escalable tanto para operadores como para usuarios finales. Se enfoca en la eficiencia, seguridad y una experiencia de usuario intuitiva.

Inspirado en sistemas como Lotto Activo, La Granjita, Lotipos y PremierPlus, este proyecto es un desafío técnico que combina interfaces dinámicas, lógica de negocio estricta y seguridad transaccional.

🎯 Demo (Proximamente)
Aquí podrás incrustar un GIF o un enlace a una demo funcional una vez que tengas algo tangible.
Visualización esperada:

Acceso con credenciales.

Selección de animales/números.

Confirmación de apuesta y generación de ticket.

Consulta de resultados.
Captura de pantalla de la interfaz principal:
`


🛠️ Tecnologías Utilizadas
Este proyecto se construye sobre un stack tecnológico moderno y robusto:

Frontend
React: Para una interfaz de usuario dinámica y componentes reutilizables.

HTML5: Estructura semántica de la aplicación.

Tailwind CSS: Para un diseño utilitario y responsivo, agilizando el desarrollo de la UI.

JavaScript (ES6+): Lógica interactiva del lado del cliente.

Fetch API: Para la comunicación asíncrona con el backend.

Metodología: Mobile-first design.

Backend
C# con ASP.NET Core Web API: Para construir un API RESTful robusta, escalable y de alto rendimiento.

Entity Framework Core: ORM para una gestión eficiente y tipada de la base de datos.

SQL Server: Base de datos relacional para almacenamiento de datos transaccionales.

SignalR: Para comunicación en tiempo real (ej. actualización de resultados de sorteos).

Pruebas y CI/CD
XUnit: Framework de testing para pruebas unitarias en C#.

TSQLT: Framework para pruebas unitarias en SQL Server, garantizando la integridad de la base de datos.

GitHub Actions: Para integración y despliegue continuo (CI/CD), automatizando el pipeline de desarrollo.

🧠 Conceptos Técnicos Aplicados
Este proyecto es un laboratorio para la aplicación de conceptos avanzados de desarrollo:

Frontend (React)
Componentización y Manejo de Estado: Gestión eficiente de la UI y el flujo de datos de apuestas utilizando React Hooks (useState, useReducer, useEffect).

CSS Grid y Flexbox: Diseño de la cuadrícula de animales y la distribución de la interfaz para una experiencia responsiva.

Validación de Formulario: Lógica de validación del lado del cliente para una UX fluida.

Backend (C# & .NET Core)
API RESTful: Diseño e implementación de endpoints REST siguiendo las mejores prácticas.

Inyección de Dependencias (DI): Gestión de servicios y componentes en ASP.NET Core.

Lógica de Negocio: Implementación de reglas estrictas para la validación de apuestas (horarios de sorteo, límites, etc.).

Gestión de Transacciones: Asegurar la atomicidad y consistencia de las operaciones en la base de datos.

Seguridad: Implementación de autenticación y autorización (JWT), y validación de datos.

Base de Datos (SQL Server)
Diseño de Esquema: Creación de tablas optimizadas para apuestas, sorteos, usuarios y transacciones.

Integridad Referencial: Uso de claves foráneas para mantener la consistencia entre las tablas.

Procedimientos Almacenados y Funciones: Optimización de operaciones complejas y lógica de negocio a nivel de base de datos.

Pruebas de Integridad: Utilización de TSQLT para asegurar que la lógica de la base de datos funciona como se espera.

DevOps
CI/CD con GitHub Actions: Automatización de la construcción, prueba y despliegue del frontend y backend.

🏗️ Arquitectura del Sistema
La arquitectura del sistema se basa en un modelo cliente-servidor con una API robusta y una base de datos centralizada.

Fragmento de código
graph TD
    A[Cliente Web/Escritorio (React)] -->|HTTP/HTTPS (Fetch)| B(ASP.NET Core Web API)
    B -->|Entity Framework Core| C[SQL Server Database]
    B -->|SignalR| A
    C -- "TSQLT Tests" --> D[GitHub Actions]
    B -- "XUnit Tests" --> D
    A -- "UI Tests" --> D
Diagrama de Arquitectura (Excalidraw):
<img width="1024" height="1024" alt="DiagramaArquitectura" src="D:\courseJune25\Proyectos\LoteriAnimalitos\img" />

