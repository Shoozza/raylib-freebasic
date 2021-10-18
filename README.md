# raylib-freebasic -> v3.7

[FreeBasic](https://freebasic.net/) bindings for [raylib](https://github.com/raysan5/raylib)  
  
platform | 
------------ | -------------
linux | works
windows | works
mac | should works
bsd | should works

## example
```basic
#include "raylib.bi"

Dim As Const Integer screen_width = 800
Dim As Const Integer screen_height = 450

InitWindow(screen_width, screen_height, "Hello World")
SetTargetFPS(60)

While Not WindowShouldClose()
	BeginDrawing()
		ClearBackground(RAYWHITE)
		DrawText("Hello World from raylib and FreeBasic!", 200, 200, 20, GRAY)
	EndDrawing()
Wend

CloseWindow()
```

![Example](example.png)
