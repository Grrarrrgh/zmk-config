This is extrapolated from my working left side only firmware. I don't have the right half of the keyboard and so cannot test further than 'Does it compile?'

The firmware is setup with both encoders and both split shifts enabled by default. To disable the encoders edit the .dtsi file to change each encoder status from "okay" to "disabled".
If not using split shifts youshould just be able to ignore the key in the keymap (maybe assign &none rather than a keycode to it?)