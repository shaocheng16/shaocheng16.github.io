---
layout: post
title:  "Calculating the 2nd force constant from LAMMPS"
categories: blog
tags: technique
data: 
---

## 2nd Force Constant From Lammps 

>In one of my  project, I need to calculate the force constant between differnet paires of atoms, and there is how I do it.  

### Methods
- The main reference is the paper from Esfarjani in 2008 [[PRB, **77**, 144112 (2018)](http://link.aps.org/doi/10.1103/PhysRevB.77.144112)]
- Basically, if we only consider the 2nd terms, the force on atom $i$ is the summation of the force between different atoms pairs:
$$F_i = - \sum_{j} \Phi_{ij} u_j$$
we can then moving one atom at each time, and the from the force of other atoms, we can calculate the force constant $\Phi_{ij}$
- In detials, I build a equilibrium lattice  in LAMMPS first, then I moved the atoms in center cell at one direction at each time, and dumped out the force on each atoms. The LAMMPS scirpts read as below:

```
group cAtom id 249
displace_atoms cAtom move 0.0 0.001 0.0 units box
dump 1 all custom 1 force_12.txt id fx fy fz
dump_modify 1 sort id format  "%d %10.15g %10.15g %10.15g"
```

- Then I used a python script to extrac the force constant between atom pairs.
- Make sure the 2nd force constants are correct, I check:
	1. the symmetry of of force constant tensor
	1. the acoustic summation rule: 
	1. the dispersion from this force constant
 