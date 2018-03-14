# localhiddenstatemodels
Data files associated to 

[General method for constructing local-hidden-variable models for entangled quantum states](https://doi.org/10.1103/PhysRevLett.117.190401)
Daniel Cavalcanti, Leonardo Guerini, Rafael Rabelo and Paul Skrzypczyk


All files are MATLAB data files (.mat) and contain the example states which are entangled but have LHS models (either for projective measurements or for POVMs).

In total there are 8 data files:

1. examples1SFIXROB.mat
2. examples1SGENROB.mat
3. examples1SRANROB.mat
4. examplesGENROB.mat
5. examplesRANROB.mat
6. examplesBSA.mat
7. examplesNEG.mat
8. examplesPOVM.mat

The first seven sets contain the examples found by from quantitative entanglement witnesses (with quantifier corresponding to the name), and contain examples which are local for all projective measurements. The last set contains the examples found which are local for all POVM measurements (using a random choice of quantatative entanglement witness).

Each of the files contains 8 variables:

Alist - 2 x 2 x 12 x n matlab array. Contains the pair of 2 x 2 matrices corresponding to the measurement operators for the 6 randomly chosen measurements for each of the n examples. The measurement operators are listed sequentially in the 3rd dimension (i.e. 1st (x=0,a=0), 2nd (x=0,a=1), 3rd (x=1,a=0), etc).

lambdalist - 1 x n matlab array. Contains the radius of the largest ball which fits inside the polytope defined by the measurement operators.

rholist - 4 x 4 x n matlab array. Contains the examples of states which are entangled and have LHS models for all projective/POVM measurements (as appropriate).

rlist - 12 x 3 x n matlab array. Contains the (x,y,z) components of the bloch vectors corresponding to each measurement operator.

slist - 1 x n matlab array. Contains the value of the associated quantifier for the example state.

Ulist - 4 x 4 x n matlab array. Contains the randomly chosen unitary matrices used to pick at random an initial entanglement witness. In particular, the first column was used to generate a random pure state of 2 qubits, and from this random pure state the optimal witness (for the given quantifer) was generated as the initial random witness.

Wlist - 4 x 4 x n matlab array. Final quantitative entanglement witness, which certifies the entanglement of the state rho, and whose value is s. 
