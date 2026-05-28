# Space Invader

Clásico juego arcade Space Invaders hecho en Python con Pygame.

## Controles

| Tecla | Acción |
|-------|--------|
| ← → | Mover la nave |
| ESPACIO | Disparar |
| R | Reintentar (en Game Over) |
| ESC | Salir (en Game Over) |

## Características

- **Sistema de olas** — 6 olas con dificultad progresiva
- **Enemigos por fases** — cada ola tiene 2 fases: primero enemigos tipo 1 (no disparan), luego tipo 2 (disparan)
- **Power-ups** que caen del cielo:
  - 🟢 **Points** — +50 puntos
  - 🔵 **Speed** — velocidad de nave aumentada temporalmente
  - 🟡 **Shield** — escudo que absorbe un golpe
- **Sistema de combo** — matar enemigos seguidos multiplica el puntaje
- **Fondo animado** — estrellas titilantes y planetas rotando
- **Efectos de sonido** — disparo, explosión y música de fondo
- **Menú principal** y pantalla de Game Over con opción de reintentar

## Instalación

```bash
pip install -r requirements.txt
python main.py
```

## Requisitos

- Python 3.8+
- pygame-ce

## Estructura del proyecto

```
SpaceInvader/
├── main.py                     # Punto de entrada
├── game.py                     # Clase Game (lógica principal)
├── entities/
│   ├── __init__.py
│   ├── background.py           # Fondo animado (estrellas, planetas)
│   ├── bullet.py               # Bala del jugador
│   ├── enemy.py                # Enemigo
│   ├── explosion.py            # Animación de explosión
│   ├── player.py               # Nave del jugador
│   └── powerup.py              # Power-ups
├── assets/
│   ├── images/                 # Sprites e imágenes
│   ├── audios/                 # Efectos de sonido y música
│   └── fonts/                  # Fuentes
├── requirements.txt
└── README.md
```
