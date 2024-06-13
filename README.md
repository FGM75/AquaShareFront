# AquaTravel
Este proyecto React implementa un mapa, mostrando sitios relacionados con el agua. Los usuarios pueden registrarse para acceder para registrar sus propios sitios.
## Funcionalidades
- Mapa: Los usuarios pueden explorar el mapa que muestra diferentes puntos relacionados con el agua.
- Registro: Los usuarios pueden registrarse para poder registrar sus propios puntos.
- PopUps: Los popups son los puntos añadidos por los usuarios donde se indica su dirección exacta y foto del lugar.

## Tecnologias Utilizadas
- React
- React Leaflet
- Firebase
- Bootstrap
- Mongo

# Diagrama de Uso

```mermaid
graph TD
    A[Inicio] -->|No está registrado| B[Registro]
    A -->|Ya está registrado| C[Inicio de Sesión]
    B --> D[Inicio de Sesión]
    C --> E[Página Principal]
    D --> E
    E -->|Agregar nuevos puntos| F[Formulario de nuevo punto]
    E -->|Ver puntos en el mapa| G[Mapa con puntos]
    G -->|Seleccionar punto| H[Detalles del punto]
    F --> G
    H -->|Volver al mapa| G
    E -->|Administrador| I[Aceptar Punto]
    I -->|Aceptar Punto| J[Bandeja de Puntos] -->|Punto Aceptado| G[Mapa con puntos]
    I -->|Denegar Punto| K[Rechazar Punto]

    style A fill:#f9f,stroke:#333,stroke-width:4px
    style E fill:#bbf,stroke:#333,stroke-width:4px
    style G fill:#bbf,stroke:#333,stroke-width:4px
    style I fill:#bbf,stroke:#333,stroke-width:4px
```

## Autor
Felipe González Muñoz
