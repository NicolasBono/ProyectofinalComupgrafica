# Parcial de Computación Gráfica 2026 — Rays

Nicolás Bono. Módulos 1 a 5: motor gráfico básico, texturas e iluminación, raycasting, raytracing por CPU y raytracing por GPU.

## Cómo correrlo

Con Python 3.13, desde la carpeta del proyecto:

```bash
python -m venv .venv
.venv/Scripts/activate        # en macOS/Linux: source .venv/bin/activate
pip install -r requirements.txt
python main.py
```

## Modos de dibujo

En `main.py`, la constante `SCENE_TYPE` elige cómo se dibuja la escena:

- `"raster"`: rasterización con texturas, Blinn-Phong y normal maps.
- `"cpu"`: raytracing en Python, a baja resolución, con sombras.
- `"gpu"` (por defecto): raytracing en la GPU con texturas, sombras y reflexiones. Usa el compute shader si hay OpenGL 4.3; si no (por ejemplo, en macOS), usa el fragment shader.

Hacer click sobre un objeto muestra u oculta su hitbox, y la consola indica qué objeto se tocó y a qué distancia.

## Capturas

Las capturas de cada paso de la guía están en `parcial/capturas`.
