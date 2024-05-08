# Chai Assertion Framework Cheatsheet

Chai is a BDD / TDD assertion library for Node.js and browsers. It provides a rich set of assertion styles and plugins.

## Installation

You can install Chai using npm or yarn:

```bash
npm install chai

yarn add chai

Assertion Styles
Chai provides three assertion styles: assert, expect, and should.
const assert = require('chai').assert;

assert.equal(actual, expected, [message]);
assert.strictEqual(actual, expected, [message]);
assert.deepEqual(actual, expected, [message]);
assert.isAbove(valueToCheck, valueToBeAbove, [message]);
assert.isBelow(valueToCheck, valueToBeBelow, [message]);
assert.isTrue(value, [message]);
assert.isFalse(value, [message]);
// and many more...

const expect = require('chai').expect;

expect(actual).to.equal(expected);
expect(actual).to.be.above(valueToBeAbove);
expect(actual).to.be.below(valueToBeBelow);
expect(value).to.be.true;
expect(value).to.be.false;
// and many more...

const should = require('chai').should();

actual.should.equal(expected);
actual.should.be.above(valueToBeAbove);
actual.should.be.below(valueToBeBelow);
value.should.be.true;
value.should.be.false
