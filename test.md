# Project 5 : Piano

## {Introduction @unplugged}

**Transform your Microbit into a Piano ! **

![Description of Image](https://edusharks.github.io/microbit_test/static/Piano.gif)

Turn your Microbit into a fun piano !
 
By using buttons and a buzzer, you can play different musical notes. Pressing a button changes the sound, letting you create your own tunes. It's a cool way to explore music and learn about technology ! 


## {Components @unplugged}

![Cartoon of the Rock Paper Scissors game](https://edusharks.github.io/microbit_test/static/CN.png)


## {Connection @unplugged}

** Connections **

**Step 1**  
Grab your **Microbit**, **Breadboard** and move to next Step ..
![Image 1](https://edusharks.github.io/microbit_test/static/S1.png)

```blocks
basic.forever(function () {
	
})
```

## {Step 12}

Click on the ``||variables:Variables||`` category in the Toolbox again. You'll notice that there are some new blocks that have appeared. Drag a ``||variables:set Value||`` block into the ``||Basic: forever||`` block.

```blocks
let Value = 0
basic.forever(function () {
    Value = 0
})
```



## {Step 13}

Click on the ``||math:Math||`` category in the Toolbox. Drag a ``||math:pick random||`` block and drop it into the ``||variables:set hand||`` block replacing the number 0. Now when we shake our micro:bit, the variable hand will contain a random number between 1 and 3.

```blocks
let hand = 0;
input.onGesture(Gesture.Shake, function() {
    hand = randint(1, 3)
})
```


```template
basic.forever(function () {
	
})
```