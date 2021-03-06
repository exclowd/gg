# gg : A library for terminal based games.

`GG` is a library for creating terminal based games in python. 
Complete with an abstraction over handling the terminal, you can decalare objects
and place then anywhere over the terminal area. There is a complete sample of a brick
breaker game provided. However this does not rely on any curses implementation, so some features may be missing.

## Major classes
The following interfaces have been created. `Scene` class helps to abstract a layout
as it maintains ownership of all the objects. A typical usage for a `Scene` might be analogous to 
that of a level. The Base class that can be added to a `Scene` is that of `Entity`. 

## Documentation
![class diagram](https://i.imgur.com/qaYpdbd.png)
### `Color`
The Color class support `256*256*256` color values.
### `Scene`
The `Scene` base class acts as a controller for all the objects to be displayed on a screen.
A game may contain multiple scenes, Eg. One for the HUD and one for the actual gameplay. Scenes may overlap.
### Surface
The `Surface` class refers to a rectangle to be blitted onto the screen
### Sprite
The `Sprite` class contstrains the `Surface` class with a predefined sprite layer for each of the characters.

## Installation
Use pip to install
```bash
pip install gg-abakfja
```