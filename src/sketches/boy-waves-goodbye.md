I lost the original ChatGPT message because I was using the VSCode extension for this experiment.

In short, I asked for an animated SVG of a boy saying goodbye to his mother as he leaves for school in the morning.

This code was quite broken, and I was unable to get ChatGPT to find it's mistakes. It created a TypeError at first
by selecting the boy circle by using querySelector on the cy attribute value. I replaced this with the use of ids.

It then tried to use getAttribute to set the posY to the cy attribute of the boy circle. I swapped this for
setAttribute.

It was trying to use textContent directly on the boy and mum rect elements. I had to replace that code with a
g element containing the rect element and a text element and provide ids on the text elements.

It did suggest using SMIL as well.