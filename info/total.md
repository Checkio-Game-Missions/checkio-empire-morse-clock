"I'm sending our time logs for the last expedition to HQ, but whith this equipment it's no easy task..."
the pilot grumbled. "Can you imagine that with all the computer power at our disposal,
I STILL have to convert this message to Morse-code using only an on/off button... Hrmph... what a colossal pain."

You will create a module for converting a normal time string to a morse time string.
As you can see in the illustration, a gray circle means on, while a white circle means off.
Every digit in the time string contains a different number of slots.
The first digit for the hours has a length of 2 while the second digit for the hour has a length of 4.
The first digits for the minutes and seconds have a length of 3 while the second digits for the minutes and
seconds have a length of 4.
Every digit in the time is converted to binary representation.
You will convert every on (or 1) signal to dash ("-") and every off (or 0) signal to dot (".").

![MorseClock](morse_clock.svg)

A time string can be in any of the following formats: _"hh:mm:ss"_, _"h:m:s"_ or _"hh:m:ss"_.
The "missing" digits are zeroes. For example, "1:2:3" is the same as "01:02:03".

The result will be a morse time string with specific format:
`h h : m m : s s`
where each digits is represented as sequence of "." and "-" (dots and dashes).

**Input:** A normal time string as a string. 

**Output:** The morse time string as a string.

**Example:**

```python
morse_time("10:37:49") == ".- .... : .-- .--- : -.. -..-"
morse_time("21:34:56") == "-. ...- : .-- .-.. : -.- .--."
morse_time("00:1:02") == ".. .... : ... ...- : ... ..-."
morse_time("23:59:59") == "-. ..-- : -.- -..- : -.- -..-"
```

**How it is used:**

Did you play the binary clocks mission earlier?
This can be the basis for a fun gift for any geek.
We've tried to combine the Morse code with a binary clock for this task and now you can create the new more complex binary clock, one which doesn't just tell time -- but makes morse style bips and beeps. ;-)   

**Precondition:**

_time_string_ contains correct time.
