# Modifying a Sequence

## Background

_Often, programmers find themselves filtering collections based on some criteria: maybe we want to filter out certain days in a collection of dates, or remove ineligible folks from a pool of applicants._

_We'll do something simple here: remove all numbers from a sequence that are under a given threshold._

## Task

Implement a method `removeUnder()` that will take a `List<Integer> sequence` and `Integer threshold` and will filter out anything that falls under the `threshold`. 
**Important**: make sure that a new List is returned instead of modifying the input sequence.

## Notes about the sample test cases

> `removeUnder_returnsEmpty_whenSequenceHasNoNumbers`
> 
> A sequence with no numbers in it has nothing to remove, so should return an empty List.

> `removeUnder_returnsEmpty_whenSequenceHasAllNumbersUnderThreshold`
> 
> A sequence that has all its numbers under the threshold will have those numbers all removed, leaving an empty List. This test runs removeUnder on the ArrayList [1,2,3] and gives a threshold of 4.

> `removeUnder_returnsUnchanged_whenSequenceHasNoNumbersUnderThreshold`
>
> A sequence that has none of its numbers under the threshold will have no numbers removed, leaving an unchanged List. This test runs removeUnder on the ArrayList [1,2,3] and gives a threshold of 0.

> `removeUnder_returnsUnchanged_whenSequenceHasAllNumbersOnThreshold`
>
>  A sequence consisting of only numbers on the threshold will return unchanged.

> `removeUnder_returnsOnlyNumbersUnderThreshold_whenSequenceHasMixOfNumbers`
>
>  Calls removeUnder with [5,5,1,3,1,1] and threshold 4 and expects [5,5].
