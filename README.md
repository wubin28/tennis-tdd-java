**Reload Countdown**

Status: http://varokas.github.io/tennis-tdd-java/

Here is the problem description:

In many games, the logic of firing your gun is as follows:
 
1. When the gun is loaded, pressing the fire key fires the gun
2. During a certain time period, the gun is "reloading", so re-pressing the fire key has no effect (other than maybe making a 'clicking' sound)
3. After the time period has passed, the gun may be fired again (assuming infinite-ammo..)

After giving that logic some thought, one idea is having a "Countdown clock" acting as the reload mechanism.
 
Create a helper class called Countdown with operations:

1. Stopped() - true if the countdown has stopped. This is the initial state
2. Start(seconds) - set the countdown to seconds, therefore Stopped() will return false
3. Decrease(seconds) - decrease the countdown. If time reaches (or passes!) zero, Stopped() will return true again

When developing the class, think about names. What names feel most "natural" when testing? Feel free to choose other names than Stopped, Start and Decrease, if those feel awkward when testing the class.
