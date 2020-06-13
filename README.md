# traverse-grid

visualization as a gradient https://traverse-grid.crabcyb.org/

visualization as a path https://crabcyb.org/experiment/traverse-paperjs

visualization as an animation https://crabcyb.org/experiment/traverse-animated

additional mutations can be found here https://crabcyb.org/post/traverse-mutations 

The main goals of traverse-grid are:
1. Allow iteration through a grid of data in a repeatable pre-defined sequence
2. Provide many methods to traverse through a grid of data to best solve a problem
3. Use as little code as possible while maintaining readability and flexibility

Written with no dependencies in ES6. Can be used via npm with `yarn add traverse-grid` or as a minified script available at https://unpkg.com/traverse-grid@latest/traverse-grid.min.js

The script is 11KB minified.

The package is free to use for any use. I would love to know if you use it in your project.

```
import { traverse as t } from 'traverse-grid';
t.spiral(5,5).map(({x,y}) => {});
t.snake(5,5).concatenate(t.diamond(5,5), 'horizontal').forEach(({index, point}) => {});
```

### What are its uses?

I use it at a strategy for data compression https://crabcyb.org/post/traversing-shape-up

I've used it to define an order that I draw in a Component https://crabcyb.org/experiment/traverse-draw-shapeup

It can be used to generate gradients and define paths. It could be used to create transition effects. If you find a use, let me know!
