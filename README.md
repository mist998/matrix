# matrix
Small idea inspired by the modern JS framework and the pain of CSS-ing.
It proposes a tiny framework, separating each window in a single webpage as zone/world, that their boundaries are fixed and any components inside always confined in it, as in a world they can never escape.
It is more like structuring the code and the way of thinking, and coincidently enforce some display rules to against some simple no-no visual bugs on a simple webpage.
At a more advanced stage, sacrifice the performance, isolate each window as world, and strictly disallow them to inteference each other except the uses of boundary utility.

Solid boundary may disable/disallow/block the boundary utilities, or totally not providing these to others(boundaries).
- Boundaries communication should done via boundary connector, boundaries animation may done via boundary state injector.
- Boundaries need no to placed near to each other to use boundary connector / boundary state injector.
- Boundary connector or boundary state injector shall be used within another boundary, but also allowing dev to use them outside the boundary with the role of matrix maintainer.
- Components within boundary must always overseen/handled by framework calculating its optimal size (default/definable by dev) in case the explicit sizing settings were not set, or, just in case, interrupt and disallow any attempt to help them escape their matrix.

Don't read, degenerate idea:
- Boundaries visualization may done via auto allocation of zIndex, traditional thinking of element within element may withhold, and now should be element on element but element on element could have element in it.
- Element within element should represent as a boundary chain
