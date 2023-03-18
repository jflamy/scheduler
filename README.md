# Weightlifting meet scheduling using Nested Monte Carlo Search

Experiment using NMCS to perform scheduling.

This views the schedule as a one-player game. The intent is as follows:
- an initial schedule is provided
- an initial list of athletes is provided with their categories (age groups and entry totals)
- athlete are brute-forced assigned to groups, descending from A, B to C.
- overflow sessions are used to handle athletes that do no fit naturally in a group. These contain
  athletes from several categories and would typically lift first.
  
The game is to fit the groups to the scheduled slots. The allowed game moves are moving athletes from one group
to another to improve the "score".  A game is won when all athletes are placed according to constraints.

[Read more](http://blog.leifbattermann.de/2016/06/05/nested-monte-carlo-search/)

