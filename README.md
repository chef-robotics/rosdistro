# Chef-Robotics workflow

We use this rosdistro fork to maintain control of the rosdep
resolutions, both for pinning and to add our own dependencies.

## Adding a dependency or updating from upstream

1. Create a branch with your favorite name, go through the normal 
   Pull Request flow, merge it to `master`.

2. Once the PR is merged, create a branch from this repo's `master` 
   branch with the name `r.N` where N is an increasing "version number".
  > NOTE: Once created it will be a protected branch

3. Once created, create a PR in ChefAutonomy (or whatever other repo
  that uses this) to change the branch pointed to by docker builds.
  For ChefAutonomy, also update `cheftool`.

  Example: https://github.com/chef-robotics/ChefAutonomy/pull/2896

# ros/rosdistro

This repo maintains the lists of repositories defining ROS distributions.

It is the implementation of [REP 143](http://ros.org/reps/rep-0143.html)

It also the home of the rosdep rules.

Guide to Contributing
---------------------

Please see [CONTRIBUTING.md](CONTRIBUTING.md)
