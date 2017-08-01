# LED Object Methods



### Blink

You may call the **Blink** function everywhere in the sketch. 

```c++
/* 
 * onDuration: 		The time that the pixel will stay ON in the cycle.
 * offDuration: 	The time that the pixel will stay OFF in the cycle.
 * cycles: 			The number times to repeat the ON/OFF cycle.
 * pauseDuration: 	The time that the pixel will be OFF between sequences.
 * sequences: 		The number of times to repeat the sequences.
 * callback: 		The function to call when finished.
 */
myLed.blink(onDuration, offDuration, cycles, pauseDuration, sequences, callback);
```



### On

Turn ON the LED.

```c++
/* Turn ON
 * color: 		(optional) A Color object.
 * brightness: 	(optional) A value from 0 to 255.
 */
myLed.on(color, brightness);
```



### Off

Turn OFF  the LED

```c++
// Turn OFF
myLed.off();
```



### onUntil

Turn ON the LED for a time then call a callback function.

```c++
/* onUntil 
 * onDuration: 	The time that the pixel will stay ON.
 * callback: 	The function to call when finished.
 */
myLed.onUntil(onDuration, callback);
```



### offUntil

Turn OFF the LED for a time then call a callback function.

```c++
/* offUntil
 * offDuration: The time that the pixel will stay OFF.
 * callback: 	The function to call when finished.
 */
myLed.offUntil(offDuration, callback);
```
