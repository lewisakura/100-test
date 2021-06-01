# The 100 Test
A math question that evaluates to 100. Designed to test operator precedence. 

TL;DR: `5 + 96 * 1 - 6 / 3 ^ 68 / 2 - 4 + 3 = 100`

## What is this?
The 100 Test is a simple test for programming languages and calculators alike for testing operator precedence.
When correctly evaluated, the result should equal 100 (hence its name).

A way to visualize this test as a human is by adding brackets: `5 + (96 * 1) - ((6 / (3 ^ 68)) / 2) - 4 + 3`

...or add another pair of brackets to clear up any ambiguity: `(5 + (96 * 1) - ((6 / (3 ^ 68)) / 2) - 4) + 3`

Either way, the result of this question is 100. All versions of this question should be equal to 100. If it
isn't, then something is wrong with your language/calculator's operator precedence.

## I got 66! Does that mean my language/calculator is busted?
Does your language use `^` for bitwise OR? One language that does this is Node.js. In which case, swap out `^`
for `**` since that seems to be the most common alternative for exponents. If that still doesn't work, try
looking for a `pow` function instead.

## Closing Remarks
This test was devised for [Harmony](https://github.com/ry00001/harmony), created by essentially smashing a
numpad and then tweaking it slightly to equal 100 (instead of the original 97 that it produced).

Sometimes programming languages and calculators with high precision like to make a nice large `99.99999...`
which is a completely valid answer to this! It's just that most languages round it up because the rest of
the decimal number is just `9`s.

I am not a mathemetician. I literally came up with this equation by smashing a numpad. There is probably
an edge case I haven't thought about here.
