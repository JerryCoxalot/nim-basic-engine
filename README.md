# nim-basic-engine
A simplified way of using SDL2 in the Nim programming language.

## Requirements
You must have the SDL2 wrapper for Nim installed.
Visit [the page here.](https://github.com/nim-lang/sdl2)

## Example
To open a window in this engine/framework, you'll first need to have the
engine files somewhere in your project directory. I have mine in `src/engine/*`.

```
import "src/engine/basicengine"
import "src/engine/renderer"
import "src/engine/input"
import "src/engine/basicmath"

var engine: BasicEngine

engine.basicEngineInit("Test Window", 800, 600, 60)

while engine.isRunning:
    engine.basicEngineStart()

    #[UPDATE CODE HERE]#

    #[DRAW CODE HERE]#

    engine.basicEngineEnd()
```

And there you go! A simple window that you can draw to!
