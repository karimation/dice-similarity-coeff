# dice-similarity-coeff

The Dice Similarity Coefficient is a simple and elegant way to calculate a measure of the similarity of two strings. 
The values produces are bounded between zero and one. 
The algorithm works by comparing the number of identical character pairs between the two strings.

<img src="screenshots/test.gif"  />


## Install

```bash

npm install dice-similarity-coeff --save

or 

yarn install dice-similarity-coeff

```

# Running the tests

you need to install <a href="https://facebook.github.io/jest/docs/en/22.1/getting-started.html">jest</a> 

```bash

npm test

or 

yarn test

```


# Usage

```js

import dsc from 'dice-similarity-coeff';

let result = dsc.twoStrings('Hello World', 'Hello es6'); 

```

## Examples

```js

import dsc from 'dice-similarity-coeff';
        

dsc.twoStrings('hello world','hello es6')
// 0.5
dsc.twoStrings('hello world','hello world!')
// 0.9473684210526315
dsc.twoStrings('google','facebook')
// 0.16666666666666666
dsc.twoStrings('github','microsoft')
// 1 (it is just joke result = 0)
dsc.simSort('hello',['hella','world','helloo','hel'])
// ["helloo","hella","hel","world"]

```


# Author

kerim selmi <a href="http://www.karimation.com">karimation</a>
# License

This project is licensed under the  <a href="LICENSE">MIT License</a>
