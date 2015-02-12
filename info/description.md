You will create a module for converting a normal time string to a morse time string.
As you can see in the illustration, a gray circle means on, while a white circle means off.
Every digit in the time string contains a different number of slots.
The first digit for the hours has a length of 2 while the second digit for the hour has a length of 4.
The first digits for the minutes and seconds have a length of 3 while the second digits for the minutes and
seconds have a length of 4.
Every digit in the time is converted to binary representation.
You will convert every on (or 1) signal to dash ("-") and every off (or 0) signal to dot (".").

![MorseClock](morse_clock.svg)

An time string could be in the follow formats: _"hh:mm:ss"_, _"h:m:s"_ or _"hh:m:ss"_.
The "missing" digits are zeroes. For example, "1:2:3" is the same as "01:02:03".

The result will be a morse time string with specific format:
`h h : m m : s s`
where each digits represented as sequence of "." and "-"
