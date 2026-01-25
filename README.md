# Bytebeat C Mobile

A C Bytebeat Composer optimized for mobile.

Compact calculator feel, single page, pure HTML5.

RPN VM in audio worklet.

## Interface

Two panels:
- Expression
- Keyboard

### Key layout

```text
┌───┬───┬───┬───┬───┬───────┐
│0b |0x |SR |HEX|FN |  DEL  |
├───┼───┼───┼───┼───┼───┬───┤
│ 7 | 8 | 9 | - | + | % | ~ |
├───┼───┼───┼───┼───┼───┼───┤
│ 4 | 5 | 6 | * | / | ^ | , |
├───┼───┼───┼───┼───┼───┼───┤
│ 1 | 2 | 3 | & | | | ? | : |
├───┼───┼───┼───┼───┼───┼───┤
│ t | 0 | . | ( | ) | < | > |
├───┴───┼───┴───┴───┼───┴───┤
│ Left  |   Play    | Right |
└───────┴───────────┴───────┘
```

The FN button allows to access predefined functions (Math module).

The SR button cycles through available sample rates (8000, 11025, 16000, 22050, 32000, 44100, 48000).

The HEX button toggles hexadecimal keyboard layout (access to a-f keys).

## Run locally

With NodeJS:

```
npx serve
```

With Python:

```
python -m http.server 8000
```
