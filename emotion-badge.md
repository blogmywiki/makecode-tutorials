
# Emotion badge
## What we're going to make @showdialog
Turn your micro:bit into an emotion badge, to show people around you how you're feeling.
## Clear the workspace
Delete the ``||basic: on start||`` and ``||basic: forever||`` blocks.
## Use a button to make something happen 
Add an ``||input:on button A pressed||`` block from Input.
```blocks
input.onButtonPressed(Button.A, function ()
```
    
## Add an image @showhint
Snap a ``||basic:show icon||`` block from Basic inside your ``||input:on button A pressed||`` block.
```blocks
input.onButtonPressed(Button.A, function () {
    basic.showIcon(IconNames.Heart)
})
```
## Show an emotion @showhint
Change the heart in the ``||basic:show icon||`` block to a face that shows how you're feeling.
```blocks
input.onButtonPressed(Button.A, function () {
    basic.showIcon(IconNames.Happy)
})
```
## Test it out @showhint
Now test it out in the simulator by clicking or tapping on button A.
If you're happy it's working, go to the next step.
If not, try to work out what's wrong and fix your code.
## Add another emotion @showhint
Add or copy another ``||input:on button A pressed||`` and ``||basic:show icon||`` block and change the face to another emotion, like sad.
```blocks
input.onButtonPressed(Button.B, function () {
    basic.showIcon(IconNames.Sad)
})
```
## Challenge
See if you can add another emotion if you shake your micro:bit.
```blocks
input.onGesture(Gesture.Shake, function () {
    basic.showIcon(IconNames.Surprised)
})
```
## Finish
Now transfer the code to your micro:bit and show the world how you feel!
