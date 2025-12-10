# ZMK Config

Personal ZMK firmware configuration for Corne split keyboard.

## Build

Push to GitHub → Actions tab → Download `firmware.zip`

## Corne Layout

### Layer 0: BASE (Graphite)
```
┌─────┬─────┬─────┬─────┬─────┬─────┐       ┌─────┬─────┬─────┬─────┬─────┬─────┐
│  `  │  B  │  L  │  D  │  W  │  Z  │       │  '  │  F  │  O  │  U  │  J  │ NAV │
│  ~  │     │     │     │     │     │       │  _  │     │     │     │     │ tog │
├─────┼─────┼─────┼─────┼─────┼─────┤       ├─────┼─────┼─────┼─────┼─────┼─────┤
│     │  N  │  R  │  T  │  S  │  G  │       │  Y  │  H  │  A  │  E  │  I  │  ,  │
│     │ CTL │ ALT │ GUI │ SFT │     │       │     │ SFT │ GUI │ ALT │ CTL │  ?  │
├─────┼─────┼─────┼─────┼─────┼─────┤       ├─────┼─────┼─────┼─────┼─────┼─────┤
│     │  Q  │  X  │  M  │  C  │  V  │       │  K  │  P  │  .  │  -  │  /  │  ;  │
│     │     │     │     │ HYP │     │       │     │ HYP │  >  │  "  │  <  │  :  │
└─────┴─────┴─────┼─────┼─────┼─────┤       ├─────┼─────┼─────┼─────┴─────┴─────┘
                  │ ESC │ ENT │ TAB │       │BSPC │ SPC │⌘SPC │
                  │MEDIA│ NAV │ SYM │       │ SYM │ NUM │ FUN │
                  │  4  │  1  │  2  │       │  2  │  3  │  5  │
                  └─────┴─────┴─────┘       └─────┴─────┴─────┘
```

**Home Row Mods:** Hold N/R/T/S or H/A/E/I for CTRL/ALT/GUI/SHIFT (left) or SHIFT/GUI/ALT/CTRL (right). All mods use left keycodes. Bilateral combinations prevent misfires.

**Hyper Key:** Hold C or P for Hyper (⌃⇧⌥⌘) modifier chord. Bilateral like home row mods.

**Custom Shifts:** `'`→`_`, `,`→`?`, `-`→`"`, `/`→`<`

**Word Delete Combos:** H+A = delete prev word (⌥⌫), A+E = delete next word (⌥⌦). Word nav (⌥←/⌥→) available on NAV layer.

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

### Layer 2: SYM (TAB or BSPC)
```
┌─────┬─────┬─────┬─────┬─────┬─────┐       ┌─────┬─────┬─────┬─────┬─────┬─────┐
│     │  `  │  <  │  >  │  -  │  |  │       │  ^  │  {  │  }  │  $  │ =>  │     │
├─────┼─────┼─────┼─────┼─────┼─────┤       ├─────┼─────┼─────┼─────┼─────┼─────┤
│     │  !  │  *  │  /  │  =  │  &  │       │  #  │  (  │  )  │  ;  │  "  │     │
│     │ CTL │ ALT │ GUI │ SFT │     │       │     │ SFT │ GUI │ ALT │ CTL │     │
├─────┼─────┼─────┼─────┼─────┼─────┤       ├─────┼─────┼─────┼─────┼─────┼─────┤
│     │  ~  │  +  │  [  │  ]  │  %  │       │  @  │  :  │  ,  │  .  │  '  │     │
└─────┴─────┴─────┼─────┼─────┼─────┤       ├─────┼─────┼─────┼─────┴─────┴─────┘
                  │     │     │ ### │       │ ### │     │     │
                  └─────┴─────┴─────┘       └─────┴─────┴─────┘
```
Either thumb (TAB or BSPC) activates. Home row symbols have HRM: hold for modifier, tap for symbol.

**Arrow:** `=>` tap, `->` shift+tap.

### Layer 3: NUM (SPC)
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

### Layer 4: MEDIA (ESC)
```
┌─────┬─────┬─────┬─────┬─────┬─────┐       ┌─────┬─────┬─────┬─────┬─────┬─────┐
│     │     │     │VOL- │VOL+ │     │       │     │WH_D │ M↑  │WH_U │     │     │
├─────┼─────┼─────┼─────┼─────┼─────┤       ├─────┼─────┼─────┼─────┼─────┼─────┤
│     │STOP │PLAY │PREV │NEXT │     │       │     │ M←  │ M↓  │ M→  │     │     │
├─────┼─────┼─────┼─────┼─────┼─────┤       ├─────┼─────┼─────┼─────┼─────┼─────┤
│     │     │BRI- │BRI+ │MUTE │     │       │     │     │     │     │     │     │
└─────┴─────┴─────┼─────┼─────┼─────┤       ├─────┼─────┼─────┼─────┴─────┴─────┘
                  │ ### │     │     │       │BTN2 │BTN1 │BTN3 │
                  └─────┴─────┴─────┘       └─────┴─────┴─────┘
```
Hold ESC to access. Left: media controls (STOP/PLAY/PREV/NEXT), volume, brightness, mute. Right: mouse movement (OHAE positions), scroll (F/U), buttons on thumbs (L/M/R click).

### Layer 5: FUN (⌘SPC)
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
Hold ⌘SPC to access. F-keys mirror NUM layer positions. Right side: RGB controls (TOG/HUI/HUD/BRI/BRD/EFF) and Bluetooth profile selection (BT0-4, BTCLR).

## Flash

1. Connect keyboard half via USB
2. Double-tap reset button (enters bootloader)
3. Copy `.uf2` file to mounted USB drive
4. Repeat for other half
