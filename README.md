# Colemak-dh Dactyl Manuform Keymap

This repo serves as the basis for my current keyboard, a 5x6+3 Dactyl Manuform. My specific keyboard was designed by [Marshall from TheBigSkree](https://www.etsy.com/shop/TheBigSkree?ref=shop-header-name&listing_id=1368030922&from_page=listing) on Etsy for my specific needs. It also serves as a record for things I have tried, wanted to try, and what I am currently doing with my keyboard in case something goes awry.

# The Firmware
This keyboard runs on the [ZMK](https://zmk.dev/) firmware, and the key bindings are generated with a [GUI](https://nickcoutsos.github.io/keymap-editor/) that was created by Nick Coutsos.

Setting, creating, and modifying keys and layers is done entirely through this GUI, which is connected to this Github repo and uses it's built-in Github Actions to build and serve two .UF2 files (one for each half of the keyboard), which are then flashed on the keyboard itself.

# The Keymap
Things have changed! I was originally using a three layer system, but after taking heavy inspiration from [Suraj N. Kurapati](https://sunaku.github.io/), I am now using a 6-ishlayer system.

## Default Layer
![base](https://github.com/user-attachments/assets/a216bc58-c802-4817-84c6-ee875f42369f)

As the name suggests, this is the default layer for everyday use. I have been using [Colemak-dh](https://colemakmods.github.io/mod-dh/) for over two years now with no complaints.
My specific layout shares all the same alpha keys and symbols, with the addition of a number row at the top and typical keyboard symbols and special keys. With the additon of the 3x3 thumb clusters, we have 12 new keys to map as we see fit.

### What's up with those home rows?
I have finally converted to the churh of Home Row Mods (TM).
On my left hand, ARST are letters when *tapped*, but Meta/Alt/Ctrl/Shift when *held*. I had to modify some behaviors to make it work properly, mostly because the default hold ms isn't long enough, and I also kept rolling into multiple commands when typing several keys too quickly. Namely `quick-tap-ms`, `require-prior-middle-ms` to my preferred measurements, and `flavor` to `balanced`.

These have been a **massive** change to my productivity. I now have much better control of using and adopting new shortcuts, and I feel like I'm a hacker in an 80s movie.

### Left Thumb Cluster
This handles more complex button presses, as my dominant hand (right) is occasionally using the mouse. The top row, L-shift, Escape (hold to go to my Number layer), left/right, Tab, and Delete (held to go to the Function layer). Hold/tap is also in play here for the two layer keys, while adding Tab to the thumb has just been super nifty. I don't use Esc as much as I probably could, but it's still nifty.

### Right Thumb Cluster
Similar to the left, this has up/down and some more hold/tap layers. Space converts to my Symbol layer, Backspace held leads to the Cursor layer. Losing the ability to hold down backspace was annoying at first, but with home row mods I can easily hold Ctrl and delete whole words. The last button is not a tap layer, instead sending it to the Colemak gaming layer.

## Cursor Layer
![cursor](https://github.com/user-attachments/assets/54dbaa48-127c-4062-9850-5eb18e46806a)

This is new, again taking inspiration from Suraj. Easy access to all four arrow keys and some quick macros (copy, cut, paste, highlighting, undo/redo) give me the ability to quickly navigate and edit text. I use this layer a LOT.

## Number & Function Layer
![number](https://github.com/user-attachments/assets/72799def-16c9-40d7-aa6e-62b6ac76c265)
![func](https://github.com/user-attachments/assets/6b3bb15a-1064-4bd6-b2c8-8c1cdac465c9)

Hey guess what, it's a number pad. There's not much to say here, likewise for the function layer.

## Symbol Layer
![symbols](https://github.com/user-attachments/assets/4b75294e-35b9-44b9-b37b-2a37c09ff72c)

Now that I am coding more often, having access to special symbols is much more vital than before. Where on my previous keyboard, my second layer was a mix of symbols, a numpad, and random special functions, this one doubles-down on full symbols. This newer layout is also taken from Suraj, with some symbols swapped around purely because I couldn't beat muscle memory. 

I wouldn't be surprised if I end up changing this layer in the future, mainly to get better access to some symbols and removing lesser-used ones.

## Colemak "Gaming" Layer
![colemak](https://github.com/user-attachments/assets/75d20bab-1faa-4aec-b8d3-326a3e2fc0b3)

This is essentially the previous iteration of my base layer. It only exists because I have World of Warcraft keybindings and I don't want to completely overhaul them to play. Sorry, not sorry.

## QWERTY Layer
![qwerty](https://github.com/abrakablam/zmk-xiao-flex-v2/assets/165574894/f54fcf5f-09a8-4af2-b3db-5a486f388b7b)

Finally, we come to a completely new layer. As some 70% of the modern world uses QWERTY, it's not entirely useless to have it. The primary purpose of this layer, however, is purely for video games. While most games offer remapping controls, they are almost never implemented the same ways, and are often incredibly lacking. And for many other games. there simply just aren't any keymapping options, or they are severely limited, leading to unaccessible keys or double-mapping keys, which is a massive pain. So, instead of fighting these systems, we now have a plain QWERTY layer.
