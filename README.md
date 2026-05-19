![image alt](https://github.com/Marianoz1972/lab2026/blob/main/Imagenes/banner_qr_center.png?raw=true)

<p align="center">
  <img src="https://capsule-render.vercel.app/api?type=waving&color=0:0f172a,100:2563eb&height=220&section=header&text=LAB2026&fontSize=56&fontColor=ffffff&animation=fadeIn" alt="Banner principal de lab2026" />
</p>

Bienvenido a **lab2026** 👋


## Descripción

Este repositorio está preparado como laboratorio para pruebas, experimentación y documentación del proyecto.


## Estructura inicial

`README.md`: documentación principal del proyecto.


##   Desarrollo de aplicaciones para Maya


💡 Lighting Tool PRO

🎯 ¿Qué hace esta herramienta?

## Panel De La Herramienta

El panel principal incluye controles para:

- `Light type`: tipo de luz a crear.
- `Count`: cantidad de luces.
- `Intensity`: intensidad de las luces.
- `Color`: color de las luces.
- `Height`: altura de las luces en relacion al tamano del objeto.
- `Distance`: distancia de las luces respecto al objeto.
- `Replace previous lights`: borra las luces anteriores creadas por la herramienta antes de crear nuevas.

Tambien incluye botones para:

- `Create Lights`: crear luces con los valores elegidos.
- `Create Floor + Sky Dome`: crear el entorno basico.
- `Beauty Cameras`: crear camaras principales de presentacion.
- `Turntable Cameras`: crear camaras frontal, lateral, trasera y superior.
- `Delete Lights`: borrar luces generadas por la herramienta.
- `Delete Environment`: borrar floor y sky dome generados por la herramienta.
- `Delete Cameras`: borrar camaras generadas por la herramienta.
- `Delete All M27`: borrar todo el setup generado.

## Organizacion En Escena

Todos los objetos generados se organizan dentro de grupos con el prefijo `M27`:

## Features
- `M27_sceneSetup_GRP`: grupo principal.
- `M27_lights_GRP`: luces creadas por la herramienta.
- `M27_environment_GRP`: floor y sky dome.
- `M27_cameras_GRP`: camaras y locator de aim.

- Creates a floor and sky dome around the selected object.
- Creates lights around the selected object using themed presets:
  - Set de estudio
  - Terror
  - Interior dia
  - Exterior noche
- Creates beauty or turntable cameras aimed at the selected object.
- Deletes generated lights, environment, cameras, or the full generated setup.
- Keeps generated objects inside `M27_*` groups so cleanup does not affect unrelated scene content.
Esta organizacion permite mantener la escena limpia y borrar facilmente solo los elementos generados por la herramienta.

## Install In Maya
## Instalacion Como Modulo

1. Copy or keep the `maya2027_tool` folder somewhere stable.
2. Add the parent folder to Maya's module path, or copy `maya2027_tool.mod` into:
1. Copiar o mantener la carpeta `maya2027_tool` en una ubicacion estable.
2. Agregar la carpeta padre al module path de Maya, o copiar `maya2027_tool.mod` en:

   `Documents/maya/2027/modules`

3. Start Maya 2027.
4. Open the Script Editor and run:
3. Abrir Maya 2027.
4. Ejecutar en el Script Editor, pestaña Python:

   ```python
   import maya2027_tool
   maya2027_tool.show()
   ```

## Install Shelf Button
## Instalacion En Shelf

After the module loads, run this in Maya's Python tab:
Despues de cargar el modulo, ejecutar:

```python
import install_shelf
install_shelf.install()
```

## Development Reload
Esto crea un boton en el shelf actual para abrir la herramienta rapidamente.

Use this while editing the tool:
## Uso Recomendado

1. Seleccionar el objeto o grupo principal de la escena.
2. Crear el floor y sky dome.
3. Elegir el tipo de luz.
4. Definir cantidad, color e intensidad.
5. Crear luces.
6. Crear camaras si se necesita una vista de presentacion.
7. Ajustar manualmente las luces si se requiere un resultado mas artistico.

## Notas

- Para ver correctamente el color de las luces en el viewport, activar `Lighting > Use All Lights`.
- La herramienta no modifica el objeto seleccionado.
- Los elementos generados pueden borrarse desde los botones de cleanup.
- Si no hay ningun objeto seleccionado, la herramienta muestra una advertencia y no crea elementos.

## Estructura Del Proyecto

- `maya2027_tool.mod`: definicion de modulo de Maya.
- `scripts/maya2027_tool/main.py`: entrypoints publicos.
- `scripts/maya2027_tool/ui.py`: interfaz de usuario.
- `scripts/maya2027_tool/actions.py`: logica de creacion de luces, entorno y camaras.
- `scripts/install_shelf.py`: instalador del boton de shelf.

## Desarrollo

Durante el desarrollo, usar:

```python
import maya2027_tool.main
maya2027_tool.main.reload_and_show()
```

## Current Example Behavior

1. Select one or more transform objects in Maya.
2. Choose a theme.
3. Click `Create Themed Setup`.
4. Optionally create cameras with `Beauty Cameras` or `Turntable Cameras`.
5. Use the cleanup buttons to remove generated objects.

The tool uses the selected object's world-space bounding box to size and place the setup.
Esto recarga la herramienta y abre la ventana sin reiniciar Maya.
Escenario Inicial

![image alt](https://github.com/Marianoz1972/Tech_Art_mariano_zulueta_Porfolio/blob/9420c66e9cc0cde0a2a0e205e7c39e792170f1b4/escena%20inicial.JPG)

Herramienta en PANTALLA

![image alt](https://github.com/Marianoz1972/Tech_Art_mariano_zulueta_Porfolio/blob/6ef9d0eb211bc158bfd9a69ab1b8041d07b16c03/herramioneta%20en%20accion.JPG)

Efectos

![image alt](https://github.com/Marianoz1972/Tech_Art_mariano_zulueta_Porfolio/blob/d0ef1b21cd1802b585a534ca63e3f3ef919af91a/luz%20de%20luna.JPG)
![image alt](https://github.com/Marianoz1972/Tech_Art_mariano_zulueta_Porfolio/blob/ab61fd0ee6cf28de46f1a2e7832b6602cbcb2137/domo.JPG)

🎥 video


https://github.com/user-attachments/assets/8a3bff35-7361-4a2b-960f-1b5a1453aaa9

💥 Valor como herramienta

Esta tool no solo automatiza tareas, sino que:

👉 Estandariza calidad visual
👉 Reduce errores humanos
👉 Permite enfocarse en lo creativo


##   Enviroment en Unreal Engine


## Cómo empezar

1. Clona el repositorio.
2. Revisa este README.
3. Agrega tu código y documentación en commits pequeños y claros.





)
