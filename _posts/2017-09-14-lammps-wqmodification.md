---
layout: post
title:  "Lammps modification"
data: Thu 14 Sep 2017 04:08:56 PM EDT
categories: research
---
This year I have done a project to investigate the thermal properties of an rigid body system. 
In this project, we need to predict the thermal conductivity of this system through the Green-Kubo formula. 
From the paper by [Evans at 1976](http://www.tandfonline.com/doi/pdf/10.1080/00268977600102551), the exchange of heat flux due to the rotation of molecules need be to considered in the heat flux formula. However, we cannot access to the pairwise torque between molecules in LAMMPS right now. Therefore, I need to make some modification in Lammps to access the rotational degee-of-freedom information and get the correct heat flux information. 

