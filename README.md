# Exam clock

**This utility is in development!**

This is supposed to be a little JavaScript utility that displays:
- a clock with the current date and time, as reported on the local machine that runs this code;
- a countdown timer for a user-input amount of minutes;
- the time when the timer has been started;
- the time when the timer will stop; and
- (_optional_) additional info/reminders to students (e.g., "calculators not allowed").

I am writing this because sometimes I proctor exams.
When I do, I happen to set up a projector in the room with the following screen:

![Proof of concept](./proof_of_concept.jpg)

It is tedious to set it up everytime and it requires brain power to calculate the ending time (especially for exams that last 45, 75, etc. minutes).
Also, I do not particularly love the layout: the clock should occupy the upper half of the screen, while the countdown and the static info panel should share the lower half of the screen, especially on screens whose aspect ratio is 4:3.

This project (_finally_) gives me a bit of motivation to learn a bit of HTML, JavaScript and CSS.


## Disclaimers

You can use this code, see the [license](./LICENSE).
However, a downside of the [MIT license](https://en.wikipedia.org/wiki/MIT_License) is that I will not be responsible if you rely on this, especially for mission-critical jobs: ` THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND `.
Hence, you are encouraged to review the code before you use it.

If you have suggestions or improvements, I welcome pull requests.


## Development roadmap

- [x] code a working, self-updating clock
- [x] display current date
- [ ] code the countdown
	- [ ] allow user to specify number of minutes
	- [ ] put a button to start the timer
	- [ ] put a button to pause the timer
	- [ ] put a button to stop the timer (and track the ending time)
	- [ ] put a button to add minutes to a running timer
- [ ] display start and end times
- [ ] allow for a paragraph with additional info
- [ ] write CSS code to theme the thing
	- [x] choose a fancier font family
	- [x] choose clock & date size depending on viewport
	- [ ] choose layout depending on whether additional info is present
	- [ ] make elements' size dependent on screen real estate
	- [ ] add state-dependent cosmetics (e.g., flashing red background on timer at the end)
- [ ] bundle everything in one convenient, portable file for everyday deployment ([no, no frickin' way I'm bundling this in Electron](http://tonsky.me/blog/disenchantment/))
