# Weightlifting meet scheduling using Nested Monte Carlo Search

Experiment using NMCS to perform scheduling.

This views the schedule as a one-player game.

Creating the initial state:
- an initial schedule is provided
- an initial list of athletes is provided with their categories (age groups and entry totals)
- athlete are brute-forced assigned to groups, descending from A, B to C.
- combined overflow groups are used to handle lowest-ranked athletes from each category. These groups contain
  athletes from several categories and would typically lift first.  In medium-sized meets there could be a couple such groups with all the B athletes from the various categories.
  
Allowed moves:
 - moving athletes from one group to another
 - creating another group

The scoring function applies to legal states and makes 
- it better to have a full A group from a single category.
- it better to minimize the number of groups over which athletes are spread
- it better to have a "denser" set of entry totals


The game is to fit the groups to the scheduled slots.
A game is won when all athletes are placed according to constraints.

Open issue: can the algorithm work to find the "best" amongst winning combinations.

[Read more](http://blog.leifbattermann.de/2016/06/05/nested-monte-carlo-search/)

