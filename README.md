# star-match

In the left box, the player is challenged with a random number of stars between 1 and 9. They have to pick one or more numbers that sum to that random number of stars. If they do so correctly, the picked number(s) get marked as used (green in the UI). If they pick numbers sum to more than the random number of stars, they get marked as wrong (red in the UI). If they pick a number that is less than the random number of stars, it gets marked as selected (blue in the UI). This last case is okay because they can add more selected numbers to get to a correct answer.

There should always be a correct solution, which means the random number of stars has to depend on the remaining available numbers. If the non-used numbers are only 2 and 4, we can only challenge the player with 2, 4, or 6 stars (but still pick one of these possible values at random). This part is a bit challenging and is purely logic, so I’ll provide a ready utility function to help us with it.
