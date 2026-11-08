+++
title = 'Homework 2: Input beyond the keyboard'
draft = false
weight = 2
category = 'HCI / Homework 2'
description = 'Chris Harrison’s recent sensing work, Sutherland’s display, and surface touch in mixed reality.'
stage = 'Reading and analysis drafted'
+++

## Lecture 4 · Chris Harrison and sensing the situation

I chose [Chris Harrison](https://hcii.cmu.edu/people/chris-harrison), a professor at Carnegie Mellon University who directs the Future Interfaces Group. His work interests me because a new input method can change where an interaction happens, not just how quickly someone enters a command.

[HiFiGaze](https://www.chrisharrison.net/index.php/Research/HiFiGaze), published at CHI 2026, uses the reflection of a screen in a person's eyes. The system already knows the screen content, which helps it interpret that reflection and estimate where the person is looking. This is a useful reversal: the display becomes part of the sensing process. The research reports improved tracking over an appearance-based baseline; that does not mean every laptop camera becomes an equally reliable eye tracker.

[GazeTags](https://www.chrisharrison.net/index.php/Research/GazeTags), presented at UIST 2026, attaches small tags to objects. A narrow infrared signal from a worn device wakes tags roughly in the direction the head faces. The tags reply with an identity and potentially information about the object. It estimates attended objects through head direction, rather than recovering a precise eye-gaze point.

I see a tradeoff between those approaches. HiFiGaze extracts more from an existing camera but depends on a useful view of the eyes and their reflection. GazeTags avoids capturing images but requires objects to be instrumented. Neither makes intent obvious. Looking at a kettle could mean wanting its status, noticing its colour, or simply looking past it. A good interface should make sensing informative without treating every glance as a command.

## Lecture 5 · What I take from *The Ultimate Display*

Sutherland's [1965 paper](https://worrydream.com/refs/Sutherland%20-%20The%20Ultimate%20Display.pdf) discusses displays as ways of learning about a computer-defined world through several senses. The force-feedback example is especially useful: the user should be able to feel a simulated relationship as well as see it.

Some of that vision is familiar now. Interactive graphics let us explore impossible geometry, and tracked headsets change a view with the observer's movement. Force-feedback controls can make a simulated object resist an action. The prediction about interpreting eye movements also connects directly to today's gaze research.

I would be careful about calling all of these inventions predictions from this paper. It describes pointing and dragging systems that already existed. The larger argument is about combining capabilities and asking what kinds of experience they make possible.

My expectation is that physical props and controlled feedback will keep extending simulation. A real handle can provide weight and resistance while its virtual appearance changes. That seems more plausible in the near term than a room that generates arbitrary solid objects. A convincing image of a shelf and a shelf capable of holding a book remain different achievements.

## Lecture 6 · EclipseTouch: a table as an input surface

[EclipseTouch](https://www.chrisharrison.net/index.php/Research/EclipseTouch), a UIST 2025 research system, uses a worn camera and infrared illumination to distinguish finger hovering from surface contact. It attempts to bring touch input to ordinary surfaces without embedding a touchscreen in them.

I classify this as an optical, wearable input technique for direct spatial interaction. The user touches a surface associated with a virtual control, rather than moving a pointer with a separate mouse. The surface provides physical support and a contact cue; the tracking system decides whether the action should count.

The attractive use case is a short interaction at a desk: place a few controls on the table and rest the hand while operating them. Compared with holding a hand in the air, that could be less tiring. But “98% accuracy” reported under a study's conditions is not a guarantee that a person will experience one error in every fifty taps during ordinary use. The task, surfaces and error definition matter.

My prediction is that surface input could succeed for a small set of clear controls with visible confirmation and easy undo. I am less convinced by replacing a full keyboard. Long text needs stable key positions, reliable repeated input and low correction cost. A tracking demonstration is only the beginning of that test.
