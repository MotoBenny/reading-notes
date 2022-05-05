# MatplotLib
(I hate that name, its just not as smooth as like, pandas or numpy)

[matplotlib-tutorial](https://github.com/rougier/matplotlib-tutorial)

- matplotlib is probably the single most used Python package for 2D-graphics.

You will often need to reformat the view of your charts, for things like data outside the range, or just to change the disply slightly, There are great built in tools for all these functions.

[![figures/exercice_7.png](https://github.com/rougier/matplotlib-tutorial/raw/master/figures/exercice_7.png)](https://github.com/rougier/matplotlib-tutorial/blob/master/scripts/exercice_7.py)

Spines are the lines connecting the axis tick marks and noting the boundaries of the data area. They can be placed at arbitrary positions and until now, they were on the border of the axis. We'll change that since we want to have them in the middle. Since there are four of them (top/bottom/left/right), we'll discard the top and right by setting their color to none and we'll move the bottom and left ones to coordinate 0 in data space coordinates.

```
ax = plt.gca()
ax.spines['right'].set_color('none')
ax.spines['top'].set_color('none')
ax.xaxis.set_ticks_position('bottom')
ax.spines['bottom'].set_position(('data',0))
ax.yaxis.set_ticks_position('left')
ax.spines['left'].set_position(('data',0))
```
*we are getting dangerously close to CSS now.....*

There is quite alot here in this article. I've saved it and will absolutely be using it for reference. 