# ZMK Config

Personal ZMK firmware configuration for Corne split keyboard.

## Build

Push to GitHub → Actions tab → Download `firmware.zip`

## Corne Layout

### Layer 0: COLEMAK DH
```
┌─────┬─────┬─────┬─────┬─────┬─────┐       ┌─────┬─────┬─────┬─────┬─────┬─────┐
│  `  │  Q  │  W  │  F  │  P  │  B  │       │  J  │  L  │  U  │  Y  │  ;  │ DEL │
├─────┼─────┼─────┼─────┼─────┼─────┤       ├─────┼─────┼─────┼─────┼─────┼─────┤
│⌘SPC │  A  │  R  │  S  │  T  │  G  │       │  M  │  N  │  E  │  I  │  O  │  '  │
│     │ CTL │ ALT │ GUI │ SFT │     │       │     │ SFT │ GUI │ ALT │ CTL │     │
├─────┼─────┼─────┼─────┼─────┼─────┤       ├─────┼─────┼─────┼─────┼─────┼─────┤
│ ⌘[  │  Z  │  X  │  C  │  D  │  V  │       │  K  │  H  │  ,  │  .  │  /  │ ⌘]  │
└─────┴─────┴─────┼─────┼─────┼─────┤       ├─────┼─────┼─────┼─────┴─────┴─────┘
                  │ ESC │ ENT │ TAB │       │BSPC │ SPC │ MAG │
                  │MEDIA│ NAV │ SYM │       │ SYM │ NUM │ FUN │
                  └─────┴─────┴─────┘       └─────┴─────┴─────┘
```

**Home Row Mods:** Hold A/R/S/T or N/E/I/O for CTRL/ALT/GUI/SHIFT (left) or SHIFT/GUI/ALT/CTRL (right). All mods use left keycodes. Bilateral combinations prevent misfires.

**Hyper Key:** Hold D or H for Hyper (⌃⇧⌥⌘) modifier chord. Bilateral like home row mods.

### Layer 1: NAV
```
┌─────┬─────┬─────┬─────┬─────┬─────┐       ┌─────┬─────┬─────┬─────┬─────┬─────┐
│     │     │     │     │     │     │       │UNDO │PASTE│COPY │ CUT │REDO │     │
├─────┼─────┼─────┼─────┼─────┼─────┤       ├─────┼─────┼─────┼─────┼─────┼─────┤
│     │ CTL │ ALT │ GUI │ SFT │     │       │  ←  │  ↓  │  ↑  │  →  │     │     │
├─────┼─────┼─────┼─────┼─────┼─────┤       ├─────┼─────┼─────┼─────┼─────┼─────┤
│     │     │     │ RLD │ BCK │ FWD │       │HOME │PGDN │PGUP │ END │     │     │
└─────┴─────┴─────┼─────┼─────┼─────┤       ├─────┼─────┼─────┼─────┴─────┴─────┘
                  │     │ ### │     │       │     │     │     │
                  └─────┴─────┴─────┘       └─────┴─────┴─────┘
```

**NAV Combos:** N+E = previous word (⌥←), E+I = next word (⌥→)

### Layer 2: SYM-L (left thumb TAB)
```
┌─────┬─────┬─────┬─────┬─────┬─────┐       ┌─────┬─────┬─────┬─────┬─────┬─────┐
│     │     │     │     │     │     │       │  ^  │  &  │  |  │  @  │ =>  │     │
├─────┼─────┼─────┼─────┼─────┼─────┤       ├─────┼─────┼─────┼─────┼─────┼─────┤
│     │ CTL │ ALT │ GUI │ SFT │     │       │  #  │  ?  │  :  │  =  │  !  │  ;  │
├─────┼─────┼─────┼─────┼─────┼─────┤       ├─────┼─────┼─────┼─────┼─────┼─────┤
│     │     │     │     │     │     │       │  $  │ ??  │ ?.  │ &&  │ ||  │  ,  │
└─────┴─────┴─────┼─────┼─────┼─────┤       ├─────┼─────┼─────┼─────┴─────┴─────┘
                  │     │     │ ### │       │     │     │     │
                  └─────┴─────┴─────┘       └─────┴─────┴─────┘
```
Left thumb activates right-side symbols with left-side home row mods.

### Layer 3: SYM-R (right thumb BSPC)
```
┌─────┬─────┬─────┬─────┬─────┬─────┐       ┌─────┬─────┬─────┬─────┬─────┬─────┐
│     │  `  │  *  │  +  │  -  │  ~  │       │     │     │     │     │     │     │
├─────┼─────┼─────┼─────┼─────┼─────┤       ├─────┼─────┼─────┼─────┼─────┼─────┤
│     │  (  │  {  │  [  │  /  │  _  │       │     │ SFT │ GUI │ ALT │ CTL │     │
├─────┼─────┼─────┼─────┼─────┼─────┤       ├─────┼─────┼─────┼─────┼─────┼─────┤
│     │  )  │  }  │  ]  │  \  │  %  │       │     │     │     │     │     │     │
└─────┴─────┴─────┼─────┼─────┼─────┤       ├─────┼─────┼─────┼─────┴─────┴─────┘
                  │     │     │     │       │ ### │     │     │
                  └─────┴─────┴─────┘       └─────┴─────┴─────┘
```
Right thumb activates left-side symbols with right-side home row mods.

**Macros:** `=>` fat arrow, `??` null coalescing, `?.` optional chaining, `&&` logical and, `||` logical or.

### Layer 4: NUM
```
┌─────┬─────┬─────┬─────┬─────┬─────┐       ┌─────┬─────┬─────┬─────┬─────┬─────┐
│     │  /  │  9  │  8  │  7  │  *  │       │     │     │     │     │     │     │
├─────┼─────┼─────┼─────┼─────┼─────┤       ├─────┼─────┼─────┼─────┼─────┼─────┤
│     │  -  │  3  │  2  │  1  │  +  │       │     │ SFT │ GUI │ ALT │ CTL │     │
├─────┼─────┼─────┼─────┼─────┼─────┤       ├─────┼─────┼─────┼─────┼─────┼─────┤
│     │  X  │  6  │  5  │  4  │  %  │       │     │     │     │     │     │     │
└─────┴─────┴─────┼─────┼─────┼─────┤       ├─────┼─────┼─────┼─────┴─────┴─────┘
                  │     │  0  │  =  │       │     │ ### │     │
                  └─────┴─────┴─────┘       └─────┴─────┴─────┘
```
Hold SPC to access. Home row (1-2-3) optimized for frequent digits. X for hex input. Right-hand home row provides modifiers for modified number input.

### Layer 5: MEDIA
```
┌─────┬─────┬─────┬─────┬─────┬─────┐       ┌─────┬─────┬─────┬─────┬─────┬─────┐
│     │     │     │     │     │     │       │     │     │     │     │     │     │
├─────┼─────┼─────┼─────┼─────┼─────┤       ├─────┼─────┼─────┼─────┼─────┼─────┤
│     │     │     │     │     │     │       │     │VOL- │VOL+ │PREV │NEXT │     │
├─────┼─────┼─────┼─────┼─────┼─────┤       ├─────┼─────┼─────┼─────┼─────┼─────┤
│     │     │     │     │     │     │       │     │     │     │     │     │     │
└─────┴─────┴─────┼─────┼─────┼─────┤       ├─────┼─────┼─────┼─────┴─────┴─────┘
                  │ ### │     │     │       │MUTE │PLAY │     │
                  └─────┴─────┴─────┘       └─────┴─────┴─────┘
```
Hold ESC to access. Volume and track controls on right home row, mute/play on right thumbs.

### Layer 6: FUN
```
┌─────┬─────┬─────┬─────┬─────┬─────┐       ┌─────┬─────┬─────┬─────┬─────┬─────┐
│     │ F12 │ F9  │ F8  │ F7  │     │       │ TOG │ HUI │ HUD │ BRI │ BRD │ EFF │
├─────┼─────┼─────┼─────┼─────┼─────┤       ├─────┼─────┼─────┼─────┼─────┼─────┤
│     │ F10 │ F3  │ F2  │ F1  │     │       │     │     │     │     │     │     │
├─────┼─────┼─────┼─────┼─────┼─────┤       ├─────┼─────┼─────┼─────┼─────┼─────┤
│     │ F11 │ F6  │ F5  │ F4  │     │       │BTCLR│ BT0 │ BT1 │ BT2 │ BT3 │ BT4 │
└─────┴─────┴─────┼─────┼─────┼─────┤       ├─────┼─────┼─────┼─────┴─────┴─────┘
                  │     │     │     │       │     │     │ ### │
                  └─────┴─────┴─────┘       └─────┴─────┴─────┘
```
Hold Magic key to access. F-keys mirror NUM layer positions. Right side: RGB controls (TOG/HUI/HUD/BRI/BRD/EFF) and Bluetooth profile selection (BT0-4, BTCLR).

## Magic Key

The right thumb key (tap) is a context-aware "magic" key using [zmk-adaptive-key](https://github.com/urob/zmk-adaptive-key). It outputs different results based on the last key pressed. Fallback is normal repeat.

### Navigation Reversals
| After | Magic outputs |
|-------|---------------|
| ← | → |
| → | ← |
| ↑ | ↓ |
| ↓ | ↑ |
| Home | End |
| End | Home |
| PgUp | PgDn |
| PgDn | PgUp |
| Bspc | Del |
| Del | Bspc |

### Bracket Pairs
| After | Magic outputs |
|-------|---------------|
| `[` | `]` |
| `]` | `[` |
| `{` | `}` |
| `}` | `{` |
| `(` | `)` |
| `)` | `(` |

### Text Completions (Magic Sturdy inspired)
| After | Magic outputs | Example |
|-------|---------------|---------|
| A | ND | a**nd** |
| B | ECAUSE | b**ecause** |
| C | Y | c**y**cle |
| D | Y | d**y**namic |
| E | U | e**u**ro |
| G | Y | g**y**m |
| I | NG | i**ng** |
| J | UST | j**ust** |
| K | S | k**s** |
| M | ENT | m**ent**al |
| N | ION | n**ion** (union) |
| O | A | o**a**k |
| P | Y | p**y**thon |
| T | MENT | t**ment** (treatment) |
| U | E | u**e** (true) |
| V | ER | v**er**y |
| W | OULD | w**ould** |
| X | ES | x**es** (boxes) |
| Y | OU | y**ou** |
| `,` | ` AND` | **, and** |
| `=` | `>` | `=>` |

**Note:** Magic completions replace normal repeat for mapped keys. Unmapped keys (F, H, L, Q, R, S, Z, numbers, etc.) still repeat normally.

## Flash

1. Connect keyboard half via USB
2. Double-tap reset button (enters bootloader)
3. Copy `.uf2` file to mounted USB drive
4. Repeat for other half
