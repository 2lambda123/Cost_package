![](http://i.imgur.com/K4OqD7N.png)

Web page : http://github.com/LCPQ/Cost_package

The different programs need atomic integrals and molecular orbitals coming from Molcas or OpenMolcas (in the last version cost_maj.tgz).


In the whole package "cost", you can find : 
- casdi: MRCI program (MR-SDCI, MR+DDCI, MR+DDCI2, MR+S), 
- dolo: localization of orbitals,
- exsci also named casdiloc: selected MRCI (quasi linear MRCI),
- noscf: to optimize orbitals (using MR-SCI and density matrices of the states, different spin multiplicity or spatial symmetry allowed),
- faiano: to transform a basis set in an ANO form (sometimes useful for the localization)
- etc...

How to install
================
1. You have untared the cost_maj.tgz file
2. cd cost_maj
3. edit file install
   answer the questions (lines containing "???")
   (i.e. choose the F90 compiler, look also at the lapack and blas variables)
4. ./install
5. Important Note: The localisation of the cost files in the file system
   appears in some files.
   As a consequence, once you have run "install":
   - DO NOT change the name of cost directory
   - DO NOT copy the cost directory (ex cp -R cost cost2) onto another place.


People involved
===============

* Daniel Maynau
* Nadia Ben Amor
* Jose-Vicente Pitarch-Ruiz
* Antonio Monari
* Sophie Hoyau

Related Papers
==============

- **CASDI and (SC)2 size-consistency correction**

  [Size-consistent self-consistent configuration interaction from a complete active space](http://dx.doi.org/doi:10.1016/S0009-2614(98)00104-3),N. Ben Amor, D. Maynau Chem. Phys.Lett. Volume 286, Issues 3–4, 10 April 1998, Pages 211–220


- **EXSCI (CASDILOC)** 

  [Selected excitation for CAS-SDCI calculations](http://dx.doi.org/doi:10.1002/jcc.20588),Bories, B., Maynau, D. and Bonnet, M.-L. (2007), J. Comput. Chem., 28: 632–643.


  [Direct selected multireference configuration interaction calculations for large systems using localized orbitals](http://dx.doi.org/10.1063/1.3600351), N. Ben Amor, F. Bessac, S. Hoyau, D. Maynau, Journal of Chemical Physics, 2011, 135, pp.014101/1-014101/14.

  [Multi-scale multireference configuration interaction calculations for large systems using localized orbitals: Partition in zones](http://dx.doi.org/10.1063/1.4747535), C. Chang,C. Calzado, N. Ben Amor, J. Sánchez-Marín, D. Maynau, Journal of Chemical Physics, 2012, 137 (10), pp.104102/1-104102/12

- **DOLO (DO Local Orbitals)**
  [Direct generation of local orbitals for multireference treatment and subsequent uses for the calculation of the correlation energy](http://dx.doi.org/10.1063/1.1476312), Daniel Maynau, Stefano Evangelisti, Nathalie Guihéry, Carmen J. Calzado and Jean-Paul Malrieu, J. Chem. Phys. 116, 10060 (2002)


