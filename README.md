# Aventura del Héroe – Proyecto Final

## Descripción
*Aventura del Héroe* es un videojuego RPG por consola desarrollado en Python como proyecto final del curso **Fundamentos de Programación**. El jugador puede explorar, combatir enemigos, gestionar su inventario, mejorar su equipo y guardar/cargar su progreso mediante archivos JSON.  
El proyecto integra los conceptos principales aprendidos durante el curso: estructuras de control, bucles, funciones, módulos, listas, diccionarios y manejo de archivos.

## Características Principales
- Creación automática de personaje
- Exploración con eventos aleatorios
- Sistema de combate por turnos
- Inventario dinámico (armas, armaduras, escudos, pociones)
- Tienda para comprar objetos
- Equipamiento y mejora de ítems
- Sistema de niveles y estadísticas
- Guardado y carga de partidas en formato JSON
- Menú interactivo fácil de usar

## Cómo ejecutar el juego
1. Asegúrate de tener Python 3 instalado.
2. Coloca todos los archivos del proyecto en la misma carpeta:
   - `juego.py`
   - `funciones.py`
   - `init.py`
3. Ejecuta el programa usando:

```
python juego.py
```

4. Selecciona una partida existente o crea una nueva.

## Estructura del Proyecto
```
📂 ProyectoFinal/
│── juego.py            # Archivo principal
│── funciones.py        # Lógica de combate, inventario y tienda
│── init.py             # Gestión de partidas y datos iniciales
│── partidas/           # Carpeta donde se guardan los .json
│── README.md           # Este archivo
```

## Estructuras de Datos Utilizadas

### Diccionario del Personaje:
```
{
  "nombre": "Zeus",
  "nivel": 1,
  "vida_max": 100,
  "vida": 96,
  "ataque": 10,
  "defensa": 5,
  "oro": 141,
  "exp": 30,
  "exp_necesaria": 100
}
```

### Lista de Enemigos:
```
[
  {"nombre": "Slime", "vida": 30, "ataque": 5, "defensa": 2, "oro": 15, "exp": 25},
  {"nombre": "Rata gigante", "vida": 35, "ataque": 6, "defensa": 2, "oro": 18, "exp": 28}
]
```

### Inventario (lista de diccionarios):
```
[
  {"id": 1, "nombre": "Poción pequeña", "tipo": "pocion", "cura": 25, "cantidad": 5},
  {"id": 2, "nombre": "Espada básica", "tipo": "arma", "ataque": 5, "equipado": true}
]
```

## Funciones Principales

### Desde `funciones.py`:
- `explorar()`
- `pelear()`
- `subir_nivel()`
- `comprar()`
- `equipar()`
- `mejorar_item()`
- `usar_pocion()`
- `ver_personaje()`
- `ver_inventario()`
- `ver_stats()`

### Desde `init.py`:
- `crear_nueva_partida()`
- `guardar_partida()`
- `cargar_partida_archivo()`
- `lista_enemigos()`
- `items_tienda()`

### Desde `juego.py`:
- `main()`
- `menu()`

## Temas Aplicados del Curso
- Condicionales
- Bucles
- Listas y diccionarios
- Modularidad
- Funciones
- Manejo de archivos JSON
- Pensamiento lógico y diseño de flujo

## Conclusión
Este proyecto reúne todos los conocimientos aprendidos en el curso, demostrando cómo Python puede usarse para desarrollar aplicaciones completas y sistemas interactivos como un videojuego por consola.
