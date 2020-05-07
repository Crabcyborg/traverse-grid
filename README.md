# traverse-grid

The main goals of traverse-grid are:
1. Allow iteration through a grid of data in a repeatable pre-defined sequence
2. Provide many methods to traverse through a grid of data to best solve a problem
3. Use as little code as possible while maintaining readability and flexibility

Written with no dependencies in ES6. Can be used via npm with `yarn add traverse-grid` or as a minified script available at https://unpkg.com/traverse-grid@latest/traverse-grid.min.js

The script is 11KB minified.

Several of the methods are illustrated in the form of a blog post here https://crabcyb.org/post/traversing-shape-up as well as here https://crabcyb.org/post/traverse-mutations 

The package is free to use for any use. I would love to know if you use it in your project.

```
import { traverse as t } from 'traverse-grid';
t.spiral(5,5).map(({x,y}) => {});
t.snake(5,5).concatenate(t.diamond(5,5), 'horizontal').forEach(({index, point}) => {});
```
