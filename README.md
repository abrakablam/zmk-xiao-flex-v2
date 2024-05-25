# Colemak-dh Dactyl Manuform Keymap

This repo serves as the basis for my current keyboard, a 5x6+3 Dactyl Manuform. My specific keyboard was designed by [Marshall from TheBigSkree](https://www.etsy.com/shop/TheBigSkree?ref=shop-header-name&listing_id=1368030922&from_page=listing) on Etsy for my specific needs. It also serves as a record for things I have tried, wanted to try, and what I am currently doing with my keyboard in case something goes awry.

# The Firmware
This keyboard runs on the [ZMK](https://zmk.dev/) firmware, and the key bindings are generated with a [GUI](https://nickcoutsos.github.io/keymap-editor/) that was created by Nick Coutsos.

Setting, creating, and modifying keys and layers is done entirely through this GUI, which is connected to this Github repo and uses it's built-in Github Actions to build and serve two .UF2 files (one for each half of the keyboard), which are then flashed on the keyboard itself.

# The Keymap
Currently, I am only running three different key layers.

## Default Layer
![default](https://github.com/abrakablam/zmk-xiao-flex-v2/assets/165574894/9aa39870-3f1f-4aca-9250-f4af5bd2a83d)

As the name suggests, this is the default layer for everyday use. I have been using [Colemak-dh](https://colemakmods.github.io/mod-dh/) for over two years now with no complaints.
My specific layout shares all the same alpha keys and symbols, with the addition of a number row at the top and typical keyboard symbols and special keys. With the additon of the 3x3 thumb clusters, we have 12 new keys to map as we see fit.

### Left Thumb Cluster
This handles more complex button presses, as my dominant hand (right) is occasionally using the mouse. The top row, L-shift, Backspace, and a momentary layer button to send us to the symbol layer. For the bottom row, we have L-Alt, Space, and and Ctrl. 

While initially modeled to be identical to my previous Iris keyboard, with the additon of two extra thumb keys and arranging them all to be more easily accessible, changes needed to be made. This thumb mainly operates Shift, Alt, and the momentary symbol layer, as well as the additon of a Backspace, Space, and L-Ctrl. At the moment, this cluster is still being updated as I get familiar with the ergonomics of the keyboard and unlearn the muscle memory from the old keyboard.

### Right Thumb Cluster
Again taking inspiration from my Iris, this handles more common typing funcions like Backspace, Space, and Enter/Return. The new additonal keys, Up/Down Arrows and a key to send us to a QWERTY layer. These keys are mostly unused and still new, and will most likely change often. Currently, I'm considering removing the arrows in place of common punctuation, but haven't tried it yet.

## Symbol Layer
![symbols](https://github.com/abrakablam/zmk-xiao-flex-v2/assets/165574894/e28be2af-1e69-4e32-a925-8610d2ba2647)

This was an idea I came across on Reddit's [r/ErgoMechKeyboards](https://old.reddit.com/r/ErgoMechKeyboards/). Now that I am coding more often, having access to special symbols is much more vital than before. Where on my previous keyboard, my second layer was a mix of symbols, a numpad, and random special functions, this one doubles-down on full symbols. While the lack of a numpad is already noticeable, it is nowhere near as important as symbols. Plus, I frequently never used most of the special functions, so they've been eliminated.

## QWERTY Layer
![qwerty](https://github.com/abrakablam/zmk-xiao-flex-v2/assets/165574894/f54fcf5f-09a8-4af2-b3db-5a486f388b7b)

Finally, we come to a completely new layer. As some 70% of the modern world uses QWERTY, it's not entirely useless to have it. The primary purpose of this layer, however, is purely for video games. While most games offer remapping controls, they are almost never implemented the same ways, and are often incredibly lacking. And for many other games. there simply just aren't any keymapping options, or they are severely limited, leading to unaccessible keys or double-mapping keys, which is a massive pain. So, instead of fighting these systems, we now have a plain QWERTY layer.
