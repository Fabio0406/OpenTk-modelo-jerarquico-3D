# OpenTK — Modelo jerárquico 3D

Programa de consola en C# que dibuja una **letra "T" en 3D** con OpenGL (OpenTK). El objetivo de la práctica es organizar la geometría en una jerarquía de clases orientada a objetos:

```
Escenario
└── Objeto   (la "T")
    └── Parte   (superior, inferior)
        └── Cara   (frente, posterior, superior, inferior, izquierda, derecha)
            └── Vértice
```

La escena se muestra en una ventana de 800×600 con rotación continua de la cámara.

> Proyecto académico — Programación Gráfica, UAGRM (2024).

## Tecnologías

- C# / .NET Framework 4.6.1
- OpenTK 3.3.3 (OpenGL)
- Newtonsoft.Json

## Estructura

```
ConsoleApp1.sln
ConsoleApp1/
├── Program.cs          # Punto de entrada
├── Game.cs             # Ventana, armado de la escena y renderizado
└── Classes/
    ├── Escenario.cs
    ├── Objeto.cs
    ├── Parte.cs
    ├── Cara.cs
    └── Vertice.cs
```

## Requisitos

- Windows
- Visual Studio 2019 o 2022 con la carga de trabajo "Desarrollo de escritorio de .NET"
- .NET Framework 4.6.1

## Cómo ejecutar

1. Abrir `ConsoleApp1.sln` en Visual Studio.
2. Restaurar los paquetes NuGet (clic derecho en la solución → *Restaurar paquetes NuGet*). Las carpetas `packages/`, `bin/` y `obj/` no están en el repositorio: Visual Studio las genera al restaurar y compilar.
3. Ejecutar con **F5**.
