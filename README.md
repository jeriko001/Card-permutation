# Card Permutation Simulator

A simulator that counts the number of steps required to return 
a deck of n cards to its initial state under a cyclic signed 
prefix-reversal shuffle.

## How it works

Starting with n cards face up in their original order, one full 
step consists of n sub-steps. In sub-step k (k = 1, 2, ..., n), 
the top k cards are physically reversed as a block: their order 
is inverted and each card is flipped (face-up becomes face-down 
and vice versa). The simulator counts how many full steps are 
required for the deck to return exactly to the initial state: 
same order and all cards face up.

## Example

For n=3, starting with [1↑, 2↑, 3↑]:
- Step 1: flip top 1 → flip top 2 → flip top 3
- Step 2: flip top 1 → flip top 2 → flip top 3
- Step 3: flip top 1 → flip top 2 → flip top 3 → back to initial state

Thus a(3) = 3 full steps = 9 sub-steps.

## Sequence

This sequence has been submitted to the 
On-Line Encyclopedia of Integer Sequences (OEIS) as A395069.

1, 8, 9, 24, 50, 72, 28, 64, 162, 60, 121, 240, 234, 392, 75, 400, ...

Verified manually and computationally up to n=20.

## Usage

Open `index.html` in any browser. No installation required. At link: https://jeriko001.github.io/Card-permutation

## Author

Fabio Longo
