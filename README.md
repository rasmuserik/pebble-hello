# pebble-hello 

Experiments with cross-platform coding, and getting back into coding C.

Development targets:

- primary
    - pebble phone (approx 22K memory available)
    - emscripten (run the code in a web browser)
- secondary
    - desktop/sdl-linux (my dev environment)
    - android
    - iOS

## Looking into build systems

Pebble uses http://waf.io/ as a build tool, - this is the source of the `wscript`-file.

cmake seems like a good build tool for general building - project is defined in CMakeLists.txt - feels much simpler/easier than old-school m4/configure-macros.

## Desired outcome

easy build + deploy:

- makes index.html+js to make it executable in browser
- deployable to watch via api

cross-platform:

- graphics
    - simple text screen (example: 4x8 font, 36x21 chars / 18x18double-chars + three lines) 
- input
    - uniform access to button-events (emulated via touch in web without buttons)

```
 123456789012345678901234567890123456
1
2
3
4
5
6
7
8
9
0
1
2
3
4
5
6
7
8
9
0
1
```
