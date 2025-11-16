# Strudelings

<b>Groups strudle drum smaples by sound type</b>

Strudel is a JavaScript synth: https://strudel.cc

Strudel comes pre-loaded with a ton of drum machine samples,</br>
however selecting the right sample takes time because the sounds</br>
are grouped by the machine they belong to and not by sound type.

In order to ease the process of selecting a particular sound,</br>
I've made arrays for each sound containing all kicks, hats, etc.

This way one can cycle through all the available kick in order</br>
to pick the perfect one instead of looking for them kit by kit. 

I've also taken the liberty to categorize the sounds based on</br>
my own taste, for instance wet splashy kicks that sound more</br>
like a snare are moved into a kicksnare category, rims shots</br>
that sound like clunking wood are put into wooden section.

To use the arrays you need to create your own drum kit:

```javascript
let drums = {
  kick:  kicks[5],
  hat:   hats[12],
  snare: snares[44],
}
```
Then use your kit in the following format:

```javascript
"<kick hat kick hat*2 kick snare ~ >*8".pickRestart(drums).sound();
```
