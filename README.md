# <center><p style="color:green;"><u>¡Guía digital de senderismo!</u></p><pre><img src="https://cdn.pixabay.com/photo/2023/08/19/23/42/ai-generated-8201368_1280.png" width="100" height="100" alt="Posible logo de la app"></pre></center>



## 📌 Índice
1. [Sobre el Proyecto](#-sobre-el-proyecto)
2. [Objetivos](#-objetivos)
3. [Tecnologías Utilizadas](#-tecnologías-utilizadas)
4. [Recursos necesarios](#-recursos-necesarios)
4. [Funcionamiento](#-funcionamiento)
5. [Información de interés](#-información-de-interés)

***

## 🚀 Sobre el Proyecto
En este proyecto, hemos trabajado para desarrollar una aplicación móvil que sirva como una ***guía digital para rutas de senderismo***. Nuestra aplicación funciona como un mapa digital y proporciona datos de interés sobre el entorno natural. 

### <u>¿Por qué esta app?</u>
Con esta guía de senderismo digital queremos ***propulsar el turismo de nuestra región*** además de concienciar a las personas a ***preservar el entorno natural*** a través del conocimiento del mismo.

><center> La naturaleza no es un lugar para visitar. Es el hogar. -- Gary Sherman Snyder</center>

En esta primera versión de la aplicación nos centraremos en rutas por la zona de Huesca, pero se planea añadir otras rutas y regiones.

## 🎯 Objetivos
- **Desarrollar una aplicación móvil** que funcione sin conexión a internet.
- **Incluir un buscador de rutas** con información relevante (_duración, longitud, desnivel, dificultad, clima, etc._).
- **Implementar navegación GPS offline** con mapas descargables y seguimiento en tiempo real.
- **Ofrecer información sobre flora, fauna y lugares históricos cercanos.**
- **Incorporar sonidos de animales** que se pueden escuchar en la ruta.
- **Crear un sistema de gestión de usuarios** para registrar rutas completadas y planificar futuras aventuras.
- **Integrar funcionalidades opcionales online** como consulta del clima y reconocimiento de flora.

## 🛠️ Tecnologías Utilizadas

![Kotlin](https://img.shields.io/badge/Kotlin-0095D5?style=for-the-badge&logo=kotlin&logoColor=white)
![Android Studio](https://img.shields.io/badge/Android_Studio-3DDC84?style=for-the-badge&logo=android-studio&logoColor=white)
![SQLite](https://img.shields.io/badge/SQLite-003B57?style=for-the-badge&logo=sqlite&logoColor=white)
![MapLibre](https://img.shields.io/badge/MapLibre-0055A5?style=for-the-badge&logo=mapbox&logoColor=white)
![PlantNet API](https://img.shields.io/badge/PlantNet_API-34A853?style=for-the-badge&logo=google&logoColor=white)

## 🔧 Recursos Necesarios

| Tecnología              | Herramienta/Framework  |
|-------------------------|------------------------|
| Lenguaje                | Kotlin                 |
| IDE                     | Android Studio         |
| Base de Datos           | SQLite con Room        |
|                         |                        |
| Mapas Offline           | MapLibre / Mapsforge   |
| Reconocimiento de Flora | PlantNet API           |


## 📍 Funcionamiento
### Diagrama entidad relación
```mermaid
erDiagram
    USUARIO {
        string id_usuario
        string nombre
        string email
    }
    RUTA {
        string id_ruta
        string nombre
        string duracion
        string dificultad
    }
    PUNTO_INTERES {
        string id_punto
        string nombre
        string descripcion
    }
    USUARIO ||--o{ RUTA : "realiza"
    RUTA ||--o{ PUNTO_INTERES : "contiene"
```

### Ejemplo de Ruta en la Aplicación
```mermaid
journey
    title Explorando la Montaña
    section Planificación
        Buscar rutas disponibles: 5: Usuario
        Descargar mapa offline: 4: Usuario
    section En la Ruta
        Iniciar navegación GPS: 5: Usuario
        Escuchar sonidos de fauna: 4: Usuario
        Ver información de puntos de interés: 3: Usuario
```
### Diagrama de flujo
```mermaid
graph TD;
    A[Inicio] --> B{Seleccionar Ruta};
    B -->|Sí| C[Descargar Mapa Offline];
    B -->|No| D[Explorar Opciones];
    C --> E[Iniciar Recorrido];
    E --> F[Ver Puntos de Interés];
    F --> G[Finalizar Ruta];
```


## 🔍 Información de interés
📧 <i.latorre@gmail.com>

🌐 [Turismo en Huesca](https://www.huesca.es/w/oficina-de-turismo)

[![Explora el Sendero](https://img.youtube.com/vi/2S06gNTgrvY/maxresdefault.jpg)](https://www.youtube.com/watch?v=2S06gNTgrvY)

---
🚶‍♂️🌲 ¡Explora, descubre y disfruta de la naturaleza con nuestra app de senderismo! 🌿🌄

---


