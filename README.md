## Members
Russell Stewart, ECE and CPE student
rstewart02@vt.edu

## Repo Link
<a class="button is-link" href="https://magicmirror.builders/" >https://magicmirror.builders/</a>

## Photo
{% include youtube.html video="miltuOLWDFQ" %}

## Mentor
Tyler Wells

## Current Status
Awaiting approval

## Project Overview

Problem: My new phone doesn't have an aux jack and my car doesn't have bluetooth.
Solution: Give the car bluetooth. I plan to do this using some old wireless earbuds, removing the batteries and unnecessary casing pieces.

Features: Can connect from phone to car to play audio. Car buttons should work for play/pause/skip/back/reset functions that the donor earbuds support.

Constraints: I only want to dissasemble my car once, for less than a day, and I want the surgery to be minimally invasive. This means the finished prototype must have all desired functionality, work perfect before fitting it into the car, and easily make adjustments to account for how much voltage the car's head unit can actually supply. To add more rigor, industry realism, and educational value to this project, I'd also like to work on very limited materials (ideally < $5-10).

Progress: After dissecting the earbuds and probing their circuitry, I am able to feed them +5v to power them and then connect to them. Using the speaker that came in our lab-in-a-box kit, I am able to play music from my phone.

Problems:

  -It appears the earbud manufacturers worked with a constraint of no negative supply. This means that the Left and Right audio channels don't reference ground, instead, they each have 2 channels (L+ and L-, R+ and R-) used to deleiver a signal to the speaker. I'm pretty sure my car only has Left and Right with reference to ground.
  
  -Without a datasheet it will be very difficult to figure out what signal and where the signal needs to be sent for the play/pause/skip/back/reset funtionality that the earbuds support. This is done externally by pressing the buttons on the earbuds a certain number of times for a certain number of seconds. So the easiest way to implement this functionality in the car will likely be using an analog circuit that mimics these button presses. I'm also unsure if the buttons in my car will give a logic 0 or 1 when pressed, so the design needs to easily adjust either way.

Next steps:

  -Make the Left and Right signals reference ground (Differential OP-Amp?) without distortion.
  
  -Design a circuit that mimics each function's button press sequence.
  
  -Tear apart my car's dashboard, integrate the final prototype into the head unit, and reassemble the car.

## Educational Value Added

-Reverse Engineering

-Analog Circuit Design

-Audio Signals, Filters, Amplifiers

-555 Timers and Analog Circuits

-Working on a minimal BOM

## Tasks

<!-- Your Text Here. See Example above -->

## Design Decisions

<!-- Your Text Here. See Example above -->

## Design Misc

<!-- Your Text Here. See Example above -->

## Steps for Documenting Your Design Process

<!-- Your Text Here. See Example above -->

## BOM + Component Cost

<!-- Your Text Here. See Example above -->

## Timeline

<!-- Your Text Here. See Example above -->

## Useful Links

<!-- Your Text Here. See Example above -->

## Log

<!-- Your Text Here. See Example above -->
