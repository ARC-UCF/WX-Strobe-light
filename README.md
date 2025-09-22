# WX-Strobe-light
Makes a strobe light flash when a Midland WR120B gets a weather alert. Detects it via shorted contacts on 3.5 mil plug. Needs X resistors in line

Arduino outputs 5v on pins 1 and 3 to power LEDs
Arduino senses 5v on pin 5 to detect contact closure

When arduino senses contact closure, it checks again (EMI issues) and then engages the pattern which repeats indefinitely until the contacts are open again.

1 megaohm resistor placed between sense-pin and ground for voltage reasons I don't fully understand.
