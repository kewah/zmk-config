# ZMK Config

Personal ZMK firmware configuration for Corne split keyboard.

## Build

Push to GitHub → Actions tab → Download `firmware.zip`

## Corne Layout

### Layer 0: COLEMAK DH
```
┌─────┬─────┬─────┬─────┬─────┬─────┐       ┌─────┬─────┬─────┬─────┬─────┬─────┐
│C-TAB│  Q  │  W  │  F  │  P  │  B  │       │  J  │  L  │  U  │  Y  │  ;  │PROFL│
├─────┼─────┼─────┼─────┼─────┼─────┤       ├─────┼─────┼─────┼─────┼─────┼─────┤
│CTRL │  A  │  R  │  S  │  T  │  G  │       │  M  │  N  │  E  │  I  │  O  │  '  │
│     │ GUI │ ALT │ CTL │ SFT │     │       │     │ SFT │ CTL │ ALT │ GUI │     │
├─────┼─────┼─────┼─────┼─────┼─────┤       ├─────┼─────┼─────┼─────┼─────┼─────┤
│CS-TB│  Z  │  X  │  C  │  D  │  V  │       │  K  │  H  │  ,  │  .  │  /  │ ESC │
└─────┴─────┴─────┼─────┼─────┼─────┤       ├─────┼─────┼─────┼─────┴─────┴─────┘
                  │ ESC │ SPC │ TAB │       │ ENT │BSPC │ DEL │
                  │MEDIA│ NAV │ SYM │       │ SYM │ NUM │ FUN │
                  └─────┴─────┴─────┘       └─────┴─────┴─────┘
```

**Home Row Mods:** Hold A/R/S/T or N/E/I/O for GUI/ALT/CTRL/SHIFT. All mods use left keycodes. Bilateral combinations prevent misfires.

### Layer 1: NAV
```
┌─────┬─────┬─────┬─────┬─────┬─────┐       ┌─────┬─────┬─────┬─────┬─────┬─────┐
│     │     │PWIN │NWIN │     │     │       │UNDO │PASTE│COPY │ CUT │REDO │     │
├─────┼─────┼─────┼─────┼─────┼─────┤       ├─────┼─────┼─────┼─────┼─────┼─────┤
│     │ GUI │ ALT │ CTL │ SFT │     │       │  ←  │  ↓  │  ↑  │  →  │     │     │
├─────┼─────┼─────┼─────┼─────┼─────┤       ├─────┼─────┼─────┼─────┼─────┼─────┤
│     │     │     │ RLD │ BCK │ FWD │       │HOME │PGDN │PGUP │ END │     │     │
└─────┴─────┴─────┼─────┼─────┼─────┤       ├─────┼─────┼─────┼─────┴─────┴─────┘
                  │ GUI │ ### │ SPC │       │ GUI │     │ SPC │
                  └─────┴─────┴─────┘       └─────┴─────┴─────┘
```

### Layer 2: SYM
```
┌─────┬─────┬─────┬─────┬─────┬─────┐       ┌─────┬─────┬─────┬─────┬─────┬─────┐
│ TAB │  !  │  @  │  #  │  $  │  %  │       │  ^  │  &  │  *  │  (  │  )  │BSPC │
├─────┼─────┼─────┼─────┼─────┼─────┤       ├─────┼─────┼─────┼─────┼─────┼─────┤
│CTRL │     │     │     │     │     │       │  -  │  =  │  [  │  ]  │  \  │  `  │
├─────┼─────┼─────┼─────┼─────┼─────┤       ├─────┼─────┼─────┼─────┼─────┼─────┤
│SHIFT│     │     │     │     │     │       │  _  │  +  │  {  │  }  │  |  │  ~  │
└─────┴─────┴─────┼─────┼─────┼─────┤       ├─────┼─────┼─────┼─────┴─────┴─────┘
                  │ GUI │     │ SPC │       │ ENT │ ### │ ALT │
                  └─────┴─────┴─────┘       └─────┴─────┴─────┘
```

### Layer 6: PROFILE
```
┌─────┬─────┬─────┬─────┬─────┬─────┐       ┌─────┬─────┬─────┬─────┬─────┬─────┐
│ TOG │ HUI │ HUD │ BRI │ BRD │ EFF │       │     │     │     │     │     │[HLD]│
├─────┼─────┼─────┼─────┼─────┼─────┤       ├─────┼─────┼─────┼─────┼─────┼─────┤
│     │ BT0 │ BT1 │ BT2 │ BT3 │ BT4 │       │     │     │     │     │     │     │
├─────┼─────┼─────┼─────┼─────┼─────┤       ├─────┼─────┼─────┼─────┼─────┼─────┤
│     │BTCLR│     │     │     │     │       │     │     │     │     │     │     │
└─────┴─────┴─────┼─────┼─────┼─────┤       ├─────┼─────┼─────┼─────┴─────┴─────┘
                  │     │     │     │       │     │     │     │
                  └─────┴─────┴─────┘       └─────┴─────┴─────┘
```
Hold top-right key to access. BT0-4 select Bluetooth profile, BTCLR clears current profile pairing. RGB controls: TOG (toggle), HUI/HUD (hue), BRI/BRD (brightness), EFF (effect).

## Flash

1. Connect keyboard half via USB
2. Double-tap reset button (enters bootloader)
3. Copy `.uf2` file to mounted USB drive
4. Repeat for other half
