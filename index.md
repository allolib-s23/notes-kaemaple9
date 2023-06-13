# Notes from Kaede Hamada
## Demo 1
- This is a transcription of "Always With Me" ("Itsumo Nandodemo") from *Spirited Away* by Yumi Kimura.
- To play this demo,
  1. Clone [my repo](https://github.com/allolib-s23/demo1-kaemaple9).
  2. Run `./run.sh kaemaple9_demos/my_demos/kh_demo1.cpp` from the root directory.
  3. Press Enter key.
- As my first experience with allolib, this demo uses square wave (additive synthesis) demonstrated in a lecture and default graphics in order to familiarize myself with its besic features. Through this demo, I explored the ways of easily calculating the time to play each note and the length of notes based on measures and beats as well as expressing articulation to make it sound more natural. 

## Demo 2
- This is a transcription of "Praise the Lord (Da Shine)" by A$AP Rocky featuring Skepta.
- To play this demo,
  1. Clone [my repo](https://github.com/allolib-s23/demo1-kaemaple9).
  2. Run `./run.sh kaemaple9_demos/my_demos/kh_demo2.cpp` from the root directory.
  3. Press Enter key.
- This demo uses sawtooth wave (additive synthesis) and three drum sounds (kick, hihat and snare) created by [Mitchell57](https://github.com/allolib-s21/notes-Mitchell57), as a new attempt compared to demo 1 that uses a single instrument. In this demo, I focused on displaying multiple graphics for each of those four instruments by manipulating their internal trigger parameters since that was not realized at that time. I also explored the way of using custom internal trigger parameters; this demo has `beat` for hihat to display its graphic moving through four positions from left to right on the screen each time it is played.
- This demo sometimes fails to display a graphic for snare sound (but not every time the sound is played). This bug might have been inspected more and solved.
- This is meant for the second course objective: Arrange existing pieces.

## Demo 3
- This is an original piece.
- To play this demo,
  1. Clone [my repo](https://github.com/allolib-s23/demo1-kaemaple9).
  2. Run `./run.sh kaemaple9_demos/my_demos/kh_demo3.cpp` from the root directory.
  3. Press Enter key.
- This demo uses sawtooth wave (additive synthesis) with manipulated amplitude envelope and default graphics. I created it to experience sound design for making a sound like a plucked string instrument (Koto) by manipulating ASDR envelope with very short attack and longer decay. Also, I chose a Japanese traditional music scale for melody to introduce a different impression from a familiar Western music scale. In this demo, I wrote the function, `playTremolo`, to easily perform tremolo just by specifying the starting time in terms of measures and beats, the length of notes and the duration of tremolo with the frequency, amplitude, attack and decay of notes. I also incorporated ritardando by adjusting the time to play notes and using even longer decay. Thank you for motivational feedback to improve those two musical expressions!
- This is meant for the first and second course objectives: 1) Design instrumental sounds. 2) Develop software engineering techniques.

## Demo 4
- This is an original piece and extention of [demo 3](#demo-3).
- To play this demo,
  1. Clone [my repo](https://github.com/allolib-s23/demo1-kaemaple9).
  2. Run `./run.sh kaemaple9_demos/my_demos/kh_demo4.cpp` from the root directory.
  3. Press Enter key.
- This demo uses sawtooth and square waves (additive synthesis) and three drum sounds (kick, hihat and snare) created by [Mitchell57](https://github.com/allolib-s21/notes-Mitchell57). For four of those five instruments, I manipulated their ASDR envelopes; In addition to the sawtooth wave I modified in demo 3 for a plucked string instrument sound, I made kick sound heavier, snare sound like a cymbal and hihat work as snare. As for drum sounds, I adjusted their sound volumes to coordinate with the melody as well. While I made demo 3 as a piece like Japanese traditional music, I used the phrase from demo 3 to create this demo as an EDM-inspired piece. In this demo, I focused on producing a hypnotic impression as a musical expression by developing its structure centered on the repeated phrase and by exploring the use of panning feature. With this goal, I applied the parameter of panning to the graphics for wave sounds to display them moving between left and right as their corresponding sounds move in contrast to static drum graphics, to enhance its mysterious impression. Thanks to inspirational feedback, I used tremolo again with a decreasing amplitude that sounds like a echo and helped me achieve that goal!
- This demo fails to play a particular note when the piece is played for the first time after its executable is run (but it plays correctly from the scoend time). This bug might have been inspected more and solved. 
- This is meant for the third course objective: Create original pieces.
