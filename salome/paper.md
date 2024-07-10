---
title: 'SALOME: Bridging CAD, Meshing, and Visualization in Numerical Simulations'
tags:
  - numerical simulation
  - CAD
  - meshing
  - visualization
  - Python
authors:
  - name: Mohd Afeef Badri
    orcid: 0000-0002-4646-8309
    corresponding: true
    affiliation: "1," 
  - name: Erwan Adam
    affiliation: 1
  - name: Vincent Bergeaud
    affiliation: 1
  - name: Alain Buhsing
    affiliation: 1
  - name: Adrien Bruneton
    affiliation: 1
  - name: Aymeric Canton
    affiliation: 1
  - name: Nabil Ghodbane
    affiliation: 1
  - name: Anida Khizar
    affiliation: 1
  - name: Francis Kloss
    affiliation: 1
  - name: Michael Ndjinga
    affiliation: 1
  - name: Bernard Secher
    affiliation: 1
  - name: Marc Tajchman
    affiliation: 1
  - name: Christian Van Wambeke
    affiliation: 1
  - name: Guillaume Brooking
    affiliation: 1
  - name: Christophe Bourcier
    affiliation: 1
  - name: Nicolas Crouzet
    affiliation: 1
  - name: Clarisse Genrault
    affiliation: 1
  - name: Nicolas Rechatin
    affiliation: 1
  - name: Aymeric Sonolet
    affiliation: 1
  - name: Cédric Aguerre
    affiliation: 2
  - name: Jean-Philippe Argaud
    affiliation: 2
  - name: Yoann Audouin
    affiliation: 2
  - name: Thibault Autrusson
    affiliation: 2
  - name: Renaud Barate
    affiliation: 2
  - name: Guillaume Boulant
    affiliation: 2
  - name: Christian Caremoli
    affiliation: 2
  - name: Jérémy Dalphin
    affiliation: 2
  - name: Gilles David
    affiliation: 2
  - name: Jean-Pierre Ducreux
    affiliation: 2
  - name: Ivan Dutka-Malen
    affiliation: 2
  - name: Eric Fayolle
    affiliation: 2
  - name: Yvan Fournier
    affiliation: 2
  - name: Anthony Geay
    affiliation: 2
  - name: Nicolas Geimer
    affiliation: 2
  - name: Stéphane Gougeon
    affiliation: 2
  - name: Bruno Lathuilière
    affiliation: 2
  - name: Thomas Lauffenburger
    affiliation: 2
  - name: Patrick Lebailly
    affiliation: 2
  - name: Vincent Lefebvre 
    affiliation: 2
  - name: Eric Lorentz
    affiliation: 2
  - name: Raphaël Marc
    affiliation: 2
  - name: Alexandra Martin Sanchez
    affiliation: 2
  - name: Ovidiu Mircescu
    affiliation: 2
  - name: Olivier Moreau
    affiliation: 2
  - name: Dimitri Mottet
    affiliation: 2
  - name: Pascale Noyret
    affiliation: 2
  - name: Pascal Obry
    affiliation: 2
  - name: Soizic Peron
    affiliation: 2
  - name: Stéphane Ploix
    affiliation: 2
  - name: Angélique Ponçot
    affiliation: 2
  - name: Alejandro Ribes-Cortes
    affiliation: 2
  - name: Frédérique Robin
    affiliation: 2
  - name: Martine Paolillo
    affiliation: 2
  - name: Paul Rascle
    affiliation: 2
  - name: Dorothée Sénéchal
    affiliation: 2
  - name: Nicolas Tardieu
    affiliation: 2
  - name: Dominique Thai-Van 
    affiliation: 2
  - name: Martin Bernhard
    affiliation: 3
  - name: Cesar Conopoima
    affiliation: 3
  - name: Julia Dorovskikh
    affiliation: 3
  - name: Yves Fricaud
    affiliation: 3
  - name: Alexey Khromov
    affiliation: 3
  - name: Konstantin Leontev
    affiliation: 3
  - name: Frédéric Pons
    affiliation: 3
  - name: Marina Prokofieva
    affiliation: 3
  - name: Nicolas Rejneri
    affiliation: 3
  - name: Dmitrii Shvydkoi
    affiliation: 3
  - name: Ekaterina Sukhareva
    affiliation: 3
  - name: Alexey Sozinov
    affiliation: 3
affiliations:
 - name: CEA  DES, Université Paris-Saclay, 91191, Gif-sur-Yvette, France
   index: 1
 - name: EDF R&D, 91120, Palaiseau, France
   index: 2
 - name: Open Cascade, 92130 Issy-les-Moulineaux, France
   index: 3
date: 13 August 2017
bibliography: paper.bib

# Optional fields if submitting to a AAS journal too, see this blog post:
# https://blog.joss.theoj.org/2018/12/a-new-collaboration-with-aas-publishing
# aas-doi: 10.3847/xxxxx <- update this with the DOI from AAS once you know it.
# aas-journal: Astrophysical Journal <- The name of the AAS journal.
---

# Summary

SALOME is an open-source, integrated platform for numerical simulation that provides researchers and engineers with a comprehensive environment for pre-processing and post-processing tasks. SALOME's ecosystem incorporates state-of-the-art components for Computer-Aided Design (CAD), meshing, mesh adaptation, data visualization, calculation supervision, and uncertainty quantification, thereby facilitating the entire workflow of computational studies across various scientific and engineering disciplines.

The platform's modular architecture allows for seamless integration of its components, creating a cohesive environment for end-to-end simulation pipelines. Users can interact with SALOME through an intuitive graphical user interface (GUI) or via Python scripts, with full interoperability between these modes of operation. This dual-interface approach enhances both accessibility for novice users and flexibility for advanced practitioners, moreover this enables efficient automation of complex workflows.

A key feature of SALOME is its extensibility, allowing researchers and software developers to construct domain-specific applications by assembling and customizing its modules. This capability facilitates the development of tailored solutions for particular numerical simulation challenges, ranging from computational fluid dynamics to structural mechanics and beyond.

By providing a unified framework that seamlessly integrates various aspects of the simulation process, SALOME aims to enhance productivity, promote collaboration, and accelerate innovation in computational science and engineering research.

# Statement of need

Numerical simulations are indispensable in modern scientific research and engineering, enabling the study of complex phenomena that are too costly, dangerous, or impractical to investigate through physical experiments alone.  Numerical simulations allow researchers and engineers to predict system behavior, optimize designs, and gain insights into various physical processes across multiple scales. A typical simulation workflow involves several key steps: geometry creation or import, mesh generation, setting up physical models and boundary conditions, solving the problem numerically, and post-processing the results for analysis. Each of these steps often requires specialized tools and expertise. Researchers and engineers in fields of numerical simulations such as computational fluid dynamics, structural mechanics, and other multiphysics scenarios  often require a comprehensive platform that can handle various aspects of the simulation workflow. SALOME addresses this need by providing:

- Integrated parametric CAD tools for geometry creation and modification
- Advanced mesh generation capabilities for complex geometries
- Pre-processing tools for setting up simulation parameters
- Post-processing and visualization features for analyzing results
- Integrated tool for uncertainty calculations
- An extensible architecture that allows integration with external solvers

Hence by using all these modules under one roof, SALOME, it aids the workflow of numerical simulations. 

## Functionality

SALOME is built on a modular architecture, offering a comprehensive suite of tools for the entire simulation workflow. Its key components include:

1. SHAPER & GEOM: These modules form the backbone of SALOME's CAD handling capabilities. They offer:
   - Creation and modification of complex 3D geometries, interactively or via a python script 
   - Import/export  support for a wide range of CAD formats (e.g., STEP, IGES, BREP)
   - Advanced geometry cleaning and healing tools to repair imperfections
   - Powerful editing features including boolean operations, fillets, and chamfers
   - Parametric modeling for easy geometry updates
2. SMESH:  A versatile meshing module that provides:
   - Generation of high-quality meshes in 0D, 1D, 2D, and 3D, meshes can also be of higher order in nature
   - Support for various element types: hexahedral, tetrahedral, pyramids, prisms,  polyhedral, quadrangular, triangular,  and hybrid meshes
   - Multiple meshing algorithms suitable for different geometry types, different algorithms can be mixed to produce 
   - Mesh quality analysis tools and automatic mesh correction features
   - Import/export capabilities for numerous mesh formats (e.g., MED, UNV, STL) 
3. HOMARD: For adapting meshes given a input field from a numerical solution or uniformly. Meshes can also  be adapted in SMESH via specialized plugins that target mesh adaption  based on numerical simulation fields.
4. PARAVIS: For advanced data visualization based on stat-of-the-art visualization  tool ParaView that has SALOME enhances with additional plugins, with  capcity to visulize mechanical fields at quarature points, neutonics-specific plugings, capcity to load MED files. 
5. YACS: A tool for managing multidisciplinary simulations through calculation schemes which  provides a means of defining a chain or coupling of calculation codes.


The platform supports various data formats, enabling interoperability with other software tools commonly used in numerical simulation workflows.

## Impact and Reuse Potential

SALOME has been widely adopted in both academic and industrial settings, contributing to research and development in various engineering disciplines. The following list present a non-exhastive list of some recent solvers/platforms that have used SALOME:

- [Code Aster](https://code-aster.org/): @@@@CITE a parallel state-of-the-art finite element solver to solve problems in mecanics, this solver hevily relies on SALOMEs capacity to produce complex geometries, meshes, post-processing @@@@CITE.
- [Code Saturne](https://www.code-saturne.org): @archambeau2004code a parallel FVM based general purpose Computational Fluid Dynamics (CFD) software, which has been ported to SALOME c.f. @salomecfd 
- [Kartos Multiphysics](https://kratosmultiphysics.github.io/Kratos/): a parallel, multi-disciplinary FEM based simulation software @kartos, which has been ported in SALOME c.f. @kartosplugin.
- [AZTLAN platform](https://inis.iaea.org/search/searchsinglerecord.aspx?recordsFor=SingleRecord&RN=46065134): Mexican platform for analysis and design of nuclear reactors @xolocostli2022integration
- DRAGON5/DONJON5: @hebert2013dragon5  platforms for designing computational schemes dedicated to fission nuclear reactors for space  which has been ported to SALOME @hebert2014integration
- CEA APPLICATIONS: @@@@CITE

These examples make it clear, the open-source nature of SALOME encourages community contributions and adaptations for specific use cases, enhancing its reuse potential across different domains of numerical simulation. The following recent publications used SALOME as one of the components for their numerical simulations: molecular dynamics @biagooi2020effects, nuclear engineering @aydemir2019coupling, @zhang2021development, 



One of the forces of SALOME is also that we provide precompiled binaries for Linux and Windows and also a tool SAT that can assist  compilation of SALOME from scratch.  

# Acknowledgements

We would like to thank A, B, C, D, E, F. Since SALOME was an evolutive effort of 20+ years, authors would like to thank A, B, C, D for their sincerer  contributions. 

# References
