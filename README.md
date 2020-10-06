# JS30 Webcam Fun
Exercise 19 in WesBos' JavaScript30 tutorials. 

Up until now I had only had experience accessing a users Media via react Native and mobile cameras, mics etc so it was nice to see a method of doing it via the web. 

I added an additional control button to flip the screen back and forth, by setting the css transform property to 180degrees and using a toggle variable to determine which way up the screen is. 

    let flipped = false
    function transform() {
        if (flipped) {
            canvas.style.transform = 'rotateX(0deg)'
            flipped = !flipped
        } else if (!flipped) {
            canvas.style.transform = 'rotateX(180deg)'
            flipped = !flipped
        }
    }

<a href="https://nikrowedevjs30-webcam-fun.netlify.app/">Demo</a>