---
layout: exercise
topic: Functions
title: Default Arguments
language: R
---

This is a follow up to [Use and Modify]({{ site.baseurl }}/exercises/Functions-use-and-modify-R).

Allowing `a` and `b` to be passed as arguments to `get_mass_from_length()` made the function more flexible, but for some types of dinosaurs we don't have specific values of `a` and `b` and so we have to use general values that can be applied to a number of different species.

Rewrite your `get_mass_from length()` function from [Use and Modify]({{ site.baseurl }}/exercises/Functions-use-and-modify-R) so that its arguments have default values of `a = 39.9` and `b = 2.6` (the average values from [Seebacher 2001](http://www.jstor.org/stable/4524171)). Recommended that you renames the function `get_mass_from length2()` or similar to avoid confusion

1. Use this function to estimate the mass of a Sauropoda (`a = 214.44`, `b = 1.46`) that
   is 22 m long (by setting `a` and `b` when calling the function).
2. Use this function to estimate the mass of a dinosaur from an unknown taxonomic group that is 16m long.
   Only pass the function `length`, not `a` and `b`, so that the default values are used.
