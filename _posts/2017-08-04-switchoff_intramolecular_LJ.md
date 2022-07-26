---
layout: post
title:  "switch off the intramolecular nonbonded interaction"
data: Fri 04 Aug 2017 01:24:22 PM EDT
categories: research
---
When I running some simulations on ionic liqudis, I realize that may need to turn off the intramolecular nonbonding interactions.
Here are some commands in LAMMPS that can do the jobs:
- night_modify exclude molecule/intra all
- special_bonds lj/coul 0 0 0
