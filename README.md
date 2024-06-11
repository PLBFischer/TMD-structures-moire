# Exciton Binding Energies in Moire

This is a repository for a research internship I did in the summer of 2023 at the group of Prof. Imamoglu at ETH Zurich. In this project I developed a numerical simulation of the band strucutre of transition metal dichalcogenide (TMD) bilayers with moire. In addition to this, I implemented a method to solve Fredholm equations with singular kernels to find the excitonic energy levels. It contains:

main_implementation: this is the main implementation of a variational approach to find the excitonic binding energies in the presence of moire. This requires solving Fredholm equations in addition to determining the moire band structure. As a variational basis set I chose states in which electron and holes are non-interacting bloch-waves.
![cbands2](https://github.com/PLBFischer/TMD-structures-moire/assets/156535559/9f3b22c5-61df-4b77-ae50-128086f78b72)

![vbands2](https://github.com/PLBFischer/TMD-structures-moire/assets/156535559/f9e21ecc-6b53-4cde-9f03-e6861f914e31)



standard_eigensolver: in the limit of a vanishing moire potential the exciton binding energies can be calculated much quicker with a standard numerical eigensolver. This file contains the implementation of such an eigensolver.
  
variational_1s: at the beginning of the project I implemented a simpler variational approach in which I used only a 1s-wavefunction as a variational state to predict the exciton binding energy as a function of the separation of the two TMD layers in the case of no Moire. 
