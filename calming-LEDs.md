
# Calming LEDs
## What we're going to make @showdialog
Turn your micro:bit into a simple digital device to help you relax by slowing and regulating your breathing using a simple animation sequence.

## Tidy your workspace
Delete the ``||basic: on start||`` block.

## Use a button to make something happen @showhint
Snap a ``||basic:pause (ms)||`` block from Basic inside the  ``||basic: forever||`` block and change the time to 2000ms (2 seconds).
```blocks
basic.forever(function () {
    basic.pause(2000)
})
```

## Add your first image @showhint
From Basic, add a ``||basic: show LEDs||`` block and click on the middle square
to show a dot.

```blocks
basic.forever(function () {
    basic.pause(2000)
    basic.showLeds(`
        . . . . .
        . . . . .
        . . # . .
        . . . . .
        . . . . .
        `)
})
```

## Add the second image @showhint
Add another ``||basic:pause (ms)||`` block, change the time to 500ms and add a ``||basic:show icon|`` block
with a small diamond image.

```blocks
basic.forever(function () {
    basic.pause(2000)
    basic.showLeds(`
        . . . . .
        . . . . .
        . . # . .
        . . . . .
        . . . . .
        `)
    basic.pause(500)
    basic.showIcon(IconNames.SmallDiamond)
})
```


## Add the third image @showhint
Add another ``||basic:pause (ms)||`` block, change the time to 2000ms and add a ``||basic:show icon|`` block
with a large diamond image.

```blocks
basic.forever(function () {
    basic.pause(2000)
    basic.showLeds(`
        . . . . .
        . . . . .
        . . # . .
        . . . . .
        . . . . .
        `)
    basic.pause(500)
    basic.showIcon(IconNames.SmallDiamond)    
    basic.showIcon(IconNames.Diamond)
    basic.pause(2000)
})
```


## Add the fourth image @showhint
Add another ``||basic:pause (ms)||`` block, change the time to 500ms and add a ``||basic:show icon|`` block
with another small diamond image.

```blocks
basic.forever(function () {
    basic.pause(2000)
    basic.showLeds(`
        . . . . .
        . . . . .
        . . # . .
        . . . . .
        . . . . .
        `)
    basic.pause(500)
    basic.showIcon(IconNames.SmallDiamond)    
    basic.showIcon(IconNames.Diamond)
    basic.pause(2000)
    basic.showIcon(IconNames.SmallDiamond)
    basic.pause(500)
})
```

## Add the last image @showhint
Add another ``||basic: show LEDs||`` block and click on the middle square
to show a dot again.

```blocks
basic.forever(function () {
    music.playTone(262, music.beat(BeatFraction.Whole))
    basic.pause(2000)
    basic.showLeds(`
        . . . . .
        . . . . .
        . . # . .
        . . . . .
        . . . . .
        `)
    basic.pause(500)
    basic.showIcon(IconNames.SmallDiamond)    
    basic.showIcon(IconNames.Diamond)
    basic.pause(2000)
    basic.showIcon(IconNames.SmallDiamond)
    basic.pause(500)
    basic.showLeds(`
        . . . . .
        . . . . .
        . . # . .
        . . . . .
        . . . . .
        `)
})
```

## Test it out
That's all the code! Now check your animation out in the simulator.
If you're happy it's working the way you want, go to the next step.
If not, try to work out what's wrong and fix your code.


## Challenge
Modify your calming animation by changing the pause times to suit your own breathing. 
Maybe you'd like to change the pictures to different shapes?


## Finish
Now transfer the code to your micro:bit and practice some relaxation.
