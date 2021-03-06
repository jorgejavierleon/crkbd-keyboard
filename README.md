# jorgejavierleon crkbd layout
personal layout mainly for programming

## to compile 
`qmk compile`
Put Your Keyboard into DFU
`qmk flash`

## layout notes

this layout uses a standard QWERTY layout on the default layer followed by a
separate layer for symbols and numbers 

To generate the json 
`qmk c2json -kb crkbd/rev1 -km jorgejavierleon -o myjson.json ~/qmk_firmware/keyboards/crkbd/keymaps/jorgejavierleon/keymap.c`

### thumb cluster: left


### thumb cluster: right


### default layer
```text
  //,-----------------------------------------------------.                    ,-----------------------------------------------------.
          TAB,       Q,       W,       E,       R,       T,                            Y,       U,       I,       O,      P,        \,
  //|--------+--------+--------+--------+--------+--------|                    |--------+--------+--------+--------+--------+--------|
         LSFT,       A,       S,       D,       F,       G,                            H,       J,       K,       L,       ;,       ',
  //|--------+--------+--------+--------+--------+--------|                    |--------+--------+--------+--------+--------+--------|
         LCTL,       Z,       X,       C,       V,       B,                            N,       M,       ,,       .,       /,   ENTER,
  //|--------+--------+--------+--------+--------+--------+--------|  |--------+--------+--------+--------+--------+--------+--------|
                                             GUI,    MO(1),     SPC,        SPC,   MO(2),    LALT
                                      //`--------------------------'  `--------------------------'
```

### symbols layer [1]

this layer contains all of the standard symbols.  the arrow keys are mapped to
the default vi bindings for single character motion (h, j, k, l).

```text
  //,-----------------------------------------------------.                    ,-----------------------------------------------------.
          ESC,       !,       @,       {,       },       |,                            ^,       +,       =,       -,       *,        ,
  //|--------+--------+--------+--------+--------+--------|                    |--------+--------+--------+--------+--------+--------|
             ,       #,     $,         (,       ),       `,                         LEFT,    DOWN,      UP,   RIGHT,        ,   ENTER,
  //|--------+--------+--------+--------+--------+--------|                    |--------+--------+--------+--------+--------+--------|
             ,       %,       ^,       [,       ],       ~,                            _,       &,       <,       >,      \,         ,
  //|--------+--------+--------+--------+--------+--------+--------|  |--------+--------+--------+--------+--------+--------+--------|
                                             GUI,    _____,     SPC,        SPC,   MO(2),    RALT
                                      //`--------------------------'  `--------------------------'
```

### number/media layer [2]

this layer has all of the numbers and the F-keys mapped to reasonably intuitive
locations.  additionally, media controls allow for quick access to volume and
track changes.

```text
  //,-----------------------------------------------------.                    ,-----------------------------------------------------.
          ESC,      F1,      F2,      F3,      F4,      F5,                           F6,      F7,      F8,      F9,     F10,     F11,
  //|--------+--------+--------+--------+--------+--------|                    |--------+--------+--------+--------+--------+--------|
             ,       1,       2,       3,       4,       5,                            6,       7,       8,       9,       0,     F12,
  //|--------+--------+--------+--------+--------+--------|                    |--------+--------+--------+--------+--------+--------|
             ,    PREV,    PLAY,    NEXT,  VOL_DN,  VOL_UP,                             ,    MUTE,        ,        ,        ,        ,
  //|--------+--------+--------+--------+--------+--------+--------|  |--------+--------+--------+--------+--------+--------+--------|
                                             OPT,      CMD,   ENTER,        SPC,   MO(1),   MO(2)
                                      //`--------------------------'  `--------------------------'

```

