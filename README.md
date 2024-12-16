# Fruit Ninja

Fruit Ninja in **pygame** using pose estimation in **MediaPipe**.

### How to Play:

Copy this GitHub repository, and run [fruit_ninja.py](scripts/fruit_ninja.py) with Python 3.

Press the `Esc` key to exit.


### Features:
- **Fruits**:
  -   Apple 
  -   Watermelon
  -   Mango
  -   Coconut
  -   Dragonfruit
  -   Bomb 
-   Silver knife trail cuts anything it touches (cut several fruits at the same time)
-   Start menu (hands up before playing to avoid accidentally starting)
-   Preview webcam video while playing by changing the `SHOW_WEBCAM` setting in [fruit_ninja.py](https://github.com/mmbaguette/Fruit-Ninja-VR/blob/main/scripts/fruit_ninja.py)

### Dependences:
```
pip install pygame
pip install opencv-python
pip install mediapipe
```


### Pyinstaller (package game into an executable)

Make your own Fruit Ninja VR executable. Use this command inside the working directory (`Fruit-Ninja-VR` not `scripts`) to package the game into an `exe` file. 
```
pyinstaller -w --onefile --paths="PYTHON_PATH\Python39\Lib\site-packages\cv2" --collect-data mediapipe --add-data "PYTHON_PATH\Python39\Lib\site-packages\mediapipe;mediapipe" -i "images/icon.ico" scripts/fruit_ninja.py
```
Install pyinstaller if you haven't already:
```
pip install pyinstaller
```
