This is extrapolated from my working left side only firmware. I don't have the right half of the keyboard and so cannot test further than 'Does it compile?'

You should  download and flash the firmware (Actions tab -> top workflow run -> Artifacts: firmware) to test the right half of the split before making any changes.
If the the key presses result in unexpected characters/actions then I've most likely made a mistake in my assumptions when assigning the Columns in the gameroy_advanced_right.overlay file.

The firmware is setup with both encoders and both split shifts enabled by default. To disable the encoders edit the .dtsi file to change each encoder status from "okay" to "disabled".
If not using split shifts youshould just be able to ignore the key in the keymap (maybe assign &none rather than a keycode to it?)

