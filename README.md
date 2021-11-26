# Coding AudioVisuals #

I started with the idea of wanting to code some music. I am not familiar with neither working with coding or music that well. So it required watching a couple tutorials for different ways to code music eg. on gibber.cc, on sonic pi, etc. I decided to go with gibber.cc since it did not require any downloading, since everything is online, it is more accessible. I followed a couple tutorials, including learning this code, play *"Another One Bites The Dust"* by *Queen.* You can hear by entering it into the gibber.cc website. 


> s = Synth('bleep');
> s.amp = 3;
> m = Mono();
> notes = ['e3', 'e3', 'e3', 'e3', 'e3', 'e3', 'g3', 'e3', 'a3'];
> times = [1/4, 0.25, 0.45, 1/16, 1/8, 1/8, 1/7, 1/16, 0.55]
> s.play(notes, times)
> m.play(notes, times)
> d = Drums ('xoxo', 1/8)


I then experimented with making music on gibber, and tried to trasncribe someone songs into code, which proved to be quite difficult. Eventually I ended up mixing the demos available on the site to create a tune that I enjoy.

> p = Drums('xox*o-')
> p.pitch = Mouse.Y

> q = FM({ attack: ms(1) }) 
> q.index = a.out 
> q.cmRatio = Mouse.X

> q.fx.add( Delay({ time: Mouse.X, feedback: Mouse.Y }) )

> q.note.seq( ['c2','c2','c2','c3','c4'].random(), [1/4,1/8,1/16].random(1/16,2) )

> c = Drums('xoxxo-', 1/16 ) .pitch.seq( [.5,1,2,4].rnd() ) .pan.seq( Rndf(-1,1) )

> d = Pluck() .note.seq( Rndi(100,300), 1/16 ) .blend.seq( Rndf() ) .fx.add( Schizo() ) .fadeIn( 8, .75 )



Upon watching the tutorials I found out that gibber.cc could also create animation. So my mission turned towards making an animation to go with the sound I made. Gibber.cc offered so much freedom in creating and experimenting with different combinations. While testing out demos, the one that particularly stood out to me was the mouse tracking option. It made the visual fun and personal. I added a kaleidoscope effect to the coding of *Mouse trails* which created an effective and interactve visual to go with my audio.


> // You might need to click the screen for it to work.
> // Move the mouse around to create shapes.

> a = Canvas()

> a.draw = function() {
> Mouse.on()

> a.fade( .05 )
  
>  a.line(
>     Mouse.prevX,
>     Mouse.prevY,
>     Mouse.x,
>     Mouse.y
>  )
  
>  a.stroke( a.randomColor(), rndi(1,100) )
>}
>
> b = Kaleidoscope()

To conclude, I felt like the brief was inflexible and challenging at the beginning but after researching and experimenting with creative computing, I understand that coding is making a bunch of connections to create a big connection that presents as something new. I've found this learning process interesting and I feel like I've learned a lot outside my usual comfort zone. I am happy with my progress so far with creative computing and will definitely be experimenting with gibber.cc a lot more and I aim to be able to create a more original work next time, with less help from demos.

You can access the completed audio visual via this link, highlight the entire code text then press Ctrl and Enter to play, Ctrl and "." to stop :) Warning that it is quite loud and you might need to click on the screen for the mouse tracking to start working. https://gibber.cc/?path=xfterlife/publications/punnapim_cc_test1
