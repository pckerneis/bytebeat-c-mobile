# BytebeatPocket Mobile

A Bytebeat Composer optimized for mobile.

Compact calculator feel, single page, pure HTML5.

## Interface

Two panels:
- Expression
- Keyboard

### Key layout

Base

```
┌───┬───┬───┬───┬───┬───┐
│ ( | ) | [ | ] |ABC|DEL|
├───┼───┼───┼───┼───┼───┤
│ ? | : | ! | & | | | ^ |
├───┼───┼───┼───┼───┼───┤
│ 7 | 8 | 9 | < | > | = |
├───┼───┼───┼───┼───┼───┤
│ 4 | 5 | 6 | + | - | % |
├───┼───┼───┼───┼───┼───┤
│ 1 | 2 | 3 | * | / | ~ |
├───┼───┼───┼───┼───┼───┤
│ ⌂ | 0 | . | ← | → | ▸ |
└───┴───┴───┴───┴───┴───┘
```

Base+Shift

```
┌───┬───┬───┬───┬───┬───┐
│MOD|SR |V+ |V- |ABC|DEL|
├───┼───┼───┼───┼───┼───┤
│   |   |   |   |   |   |
├───┼───┼───┼───┼───┼───┤
│   |   |   | { | } | # |
├───┼───┼───┼───┼───┼───┤
│   |   |   | ; | , | $ |
├───┼───┼───┼───┼───┼───┤
│   |   |   | @ | \ | $ |
├───┼───┼───┼───┼───┼───┤
│ ⌂ |   | t | ← | → | ▸ |
└───┴───┴───┴───┴───┴───┘
```

ABC

```
┌───┬───┬───┬───┬───┬───┐
│ a | b | c | d |ABC|DEL|
├───┼───┼───┼───┼───┼───┤
│ e | f | g | h | i | j |
├───┼───┼───┼───┼───┼───┤
│ k | l | m | n | o | p |
├───┼───┼───┼───┼───┼───┤
│ q | r | s | t | u | v |
├───┼───┼───┼───┼───┼───┤
│ w | x | y | z |TAB| ↲ |
├───┼───┼───┼───┼───┼───┤
│ ⌂ |SP | _ | ← | → | ▸ |
└───┴───┴───┴───┴───┴───┘
```

ABC+Shift

```
┌───┬───┬───┬───┬───┬───┐
│ A | B | C | D |ABC|DEL|
├───┼───┼───┼───┼───┼───┤
│ E | F | G | H | I | J |
├───┼───┼───┼───┼───┼───┤
│ K | L | M | N | O | P |
├───┼───┼───┼───┼───┼───┤
│ Q | R | S | T | U | V |
├───┼───┼───┼───┼───┼───┤
│ W | X | Y | Z |   |   |
├───┼───┼───┼───┼───┼───┤
│ ⌂ |   |   | ← | → | ▸ |
└───┴───┴───┴───┴───┴───┘
```

Special keys:
- `ABC` toggle alphabetic mode
- `⌂` (shift) access secondary keys for current mode*
- `←` (left) move cursor left
- `→` (right) move cursor right
- `▸` (play) toggle play state
- `DEL` delete at caret
- `TAB` insert tab (3 spaces)
- `↲` insert new line
- `SR` enter Sample rate selection. Display prompts for sample rate, between 100 and 48000. Only digits are accepted. "Play" key to validate and leave Sample rate selection.
- `MOD` enter Mode selection. Left and right keys allow to cycle through modes ("C", "JS-uint8", "JS-int8" and "JS-float"). "Play" key to validate and live Mode selection.
- `V+` to increase volume by step of 0.1 (between 0 and 1).
- `V-` to decrease volume by step of 0.1 (between 0 and 1).

*Holding shift activates secondary key if one is defined, normal key otherwise.

## Run locally

With NodeJS:

```
npx serve
```

With Python:

```
python -m http.server 8000
```
