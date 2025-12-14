# Flippy Bird Game

A simple Flappy Bird clone built with Pygame.

## Setup Instructions

1. Create a virtual environment (optional but recommended):
   ```bash
   python -m venv .venv
   source .venv/bin/activate  # On Windows: .venv\Scripts\activate
   ```

2. Install the required dependencies:
   ```bash
   pip install -r requirements.txt
   ```

3. If you encounter font-related issues, you might need to install additional system dependencies:
   ```bash
   # On macOS with Homebrew
   brew install sdl2 sdl2_image sdl2_mixer sdl2_ttf
   
   # On Ubuntu/Debian
   sudo apt-get install libsdl2-dev libsdl2-image-dev libsdl2-mixer-dev libsdl2-ttf-dev
   ```

4. Run the game:
   ```bash
   python main.py
   ```

## How to Play

- Press SPACEBAR to make the bird jump
- Click MOUSE to pause/resume the game
- Avoid hitting the green tunnels or the ground
- Try to survive as long as possible!

## Troubleshooting

If you encounter font-related errors like:
```
NotImplementedError: font module not available
```

Try these solutions:

1. Reinstall pygame:
   ```bash
   pip uninstall pygame
   pip install pygame
   ```

2. Install pygame with specific flags:
   ```bash
   pip install pygame --no-cache-dir
   ```

3. If the issue persists, the game will now fall back to a dummy font implementation.