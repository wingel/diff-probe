An almost GHZ active differential probe
=======================================

This is the design for an active differential probe which has a
bandwidth of about 800MHz and which is useful to beyond 1GHz.

I have written some articles about the probe:
[Part&nbsp;1](http://blog.weinigel.se/2016/02/26/ghz-differential-probe.html),
[Part&nbsp;2](http://blog.weinigel.se/2016/02/28/ghz-differential-probe-2.html), and
[Part&nbsp;3](http://blog.weinigel.se/2016/03/16/ghz-differential-probe-3.html).

A few notes
===========

So far I have only built the B variant of the probe, that is, the
probe with separate OP amps for the inputs.

On variant B, the input resistors R20/R21, R28/R29 and output
resistors R30/R31 are arranged in such a way that one can use just one
resistor between the input of the first resistor to the output of the
second resistor.  That's why it says "0Ω/NF" on one of the resistors
in both pairs.

The image in [S21ProbeBW_1.png](S21ProbeBW_1.png) shows a plot of the
frequency response for variant B using LMH6702 OP-AMPs, 150Ω on R20
and R28, 220Ω on R26, R27, R37 and R38 and 1.1k on R22 and R32.  Note
that the 150Ω resistors were mounted across R20/R21 and R28/R29 and
the and 50Ω matching resistor for the output was mounted across
R30/R31.  The power supply with a LMH6702 OP-AMPs should be about 5V
and the probe should be able to measure signals up to about +/-3.3V.

If you want the probe input to be AC coupled you can mount the input
resistor in its proper position on R20 and R28 and mount a capacitor
(0.1µF might be a good starting value) on R21 and R29.  You can also
AC couple the output by mounting the 50Ω matching resistor on R30 and
a another small capacitor on R31.

License
=======

[diff-probe](https://github.com/wingel/diff-probe) by
[Christer Weinigel](mailto:christer@weinigel.se) is licensed under a
[Creative Commons Attribution 4.0 International
License](http://creativecommons.org/licenses/by/4.0/).

![CC BY](https://i.creativecommons.org/l/by/4.0/88x31.png)

The intent is to make this PCB available to anyone that finds it
useful as long as I get credit for the original design.  If you want
to use the design and have issues with the above license, please
contact me.
