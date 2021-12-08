# Chef-Robotics workflow

We use this rosdistro fork to maintain control of the rosdep
resolutions, both for pinning and to add our own dependencies.

## Adding a dependency or updating from upstream

1. Create a branch from this repo's `master` branch with your change
  with the name `r.N` where N is an increasing "version number".
  > NOTE: Once created it will be a protected branch

2. Once created, create a PR in ChefAutonomy (or whatever other repo
  that uses this) to change the branch pointed to by docker builds.

  Example: https://github.com/chef-robotics/ChefAutonomy/pull/1322

3. Once 2 is accepted and merged, merge your `r.N` branch back into
  `master`; note that dev machines will still use master as the
  reference (i.e. rolling release).

# ros/rosdistro

This repo maintains the lists of repositories defining ROS distributions.

It is the implementation of [REP 143](http://ros.org/reps/rep-0143.html)

It also the home of the rosdep rules.

Guide to Contributing
---------------------

Please see [CONTRIBUTING.md](CONTRIBUTING.md)

Review guidelines
-----------------

Please see the [review guidelines](REVIEW_GUIDELINES.md) to look at the criteria to get a pull request merged into this repository.
