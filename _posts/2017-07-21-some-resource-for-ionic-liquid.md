---
layout: post
title:  "Ionic liquids: some links and resources"
data: Fri 21 Jul 2017 12:34:05 PM EDT
categories: blog
---
## Structure
- Prepare the .xyz file
    - [structures for some common room temperature ionic liquid](https://github.com/vladislavivanistsev/RTIL-FF)
- [*packmol*](http://www.ime.unicamp.br/~martinez/packmol/home.shtml) to packing the molecules into a optimized configuration  
- Generate the topology file by Topo Tool plugin in VMD
- One [tutorial](http://paulllhuang.blogspot.com/search?q=lammps)

## Potential
- OPLS-AA/AMBER framework
    + OPLS: optimized potential for liquid simulaiton, developed by Prof. Willian L. Jorgensen in 1988.
    + [JACS 110, 1657 (1988)](http://pubs.acs.org/doi/abs/10.1021/ja00214a001)
    + [JACS 118, 11225 (1996)](http://pubs.acs.org/doi/abs/10.1021/ja9621760)
- Parameters for Bmim
    + [Lopes](http://pubs.acs.org/doi/abs/10.1021/jp0362133), 2004, Modeling Ionic Liquids Using a Systematic All-Atom Force Field
    + [Lopes](http://pubs.acs.org/doi/abs/10.1021/jp063901o), 2006, Molecular Force Field for Ionic Liquids III
    + [Bhargave](http://aip.scitation.org/doi/full/10.1063/1.2772268), 2007, Refined potential model for atomistic simulations of ionic liquid [Bmim][PF6]

## Properties and applications:
- Unique properties: 
    - low volatility 
    - high electrochemical and thermal stability
    - ionic conductivity
- Dye sensitised solar cells
    + cheaper than traditional semiconductor photovoltaics, flexible, lightweight, and may offer better performance under low light conditions[^IL_review].
    + This technology is yet to be widely comercialised, with improvements in efficiency, stability and cost still required.
    + The highest confirmed DSSC solar coversion efficiency reported to data is 11.9 % using an acetonitrilebased electrolyte, but this drops significantly upon use of an IL electrolyte. 
    + The interest in using ILs as non-volatile electrolytes in DCCSs stems from the desire to develop longer lasting devices.
        + the volativlity of traditional aprotic electrolytes is a significant issue. 
+ [Review article][Energy applications of ionic liquids](http://pubs.rsc.org/en/content/articlelanding/2014/ee/c3ee42099j#!divAbstract)
+ [Overview](http://lem.ch.unito.it/didattica/infochimica/Liquidi%20Ionici/ApplicationsMap.html#M)
 ![example]({{ site.ur1}}/assets/IL_application.png  "applications of ionic liquids")
+ [Lithium batteries](https://www.nature.com/nmat/journal/v8/n8/pdf/nmat2448.pdf)
 ![example]({{ site.ur1}}/assets/lithium_batteries_ionic-liquid.png )

## Exsiting problems?
- the widespread applications of ILs in most cases have been hampered by their liquid state.
    + The confinement of ILs into nanoporous hosts is a simple but versatile strategy to overcome this problem.
    + Nanoconfined ILs constitute a new class of composites with the intrinsic chemistries of ILs and the original functions of solid matrics.

[^IL_review]: [Energy applications of ionic liquids](http://pubs.rsc.org/en/content/articlelanding/2014/ee/c3ee42099j#!divAbstract)
