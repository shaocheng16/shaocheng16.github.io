---
layout: post
title:  "Externed Green's Function Methods"
data: 
---

## Original Atomistic Green's Function Methods 

---

- The Atomistic Green's Function methods is based on the lattice dynamics of a finite body coupled to a semi-infinite thermal reservoir.
- It used the force constant matrices to compute the atomistic Green's function of the finite body
- In the original form of the AGF, the transmission function is a summation of the transmittances of all the phonon modes for a given frequency
- The original AGF method solves the phonon transmission problem in terms of the **surface Green's functions** of the lead as well as the **coupling between the channel and the leads**.
- The phonon transmission is calculated from the retarded Green function of the center
    + Self-energy terms from coupling to the left and right lead
    + The transmission is a **summation** of all the phonon modes for a given frequency
- Caroli formula: transmission function

- Given the harmonic matrix $H$ of a **close system**, the following eigenvalue equation is satisfied:
   $$[ \omega ^ 2  I -H]  \phi  = 0$$
 - When the reservoirs or contacts are held at a constant temperature by an external heat source or sink (open system), the eigenvalue equation became to:
  $$[ (\omega^2 + i 0^+)I - H] \phi = s$$ 
  	+ here $0^+$ is a small positive infinitesimal factor that introduces damping in the open system	
 
 - The total harmonic matrix of the coupled system is:
 $$ H_{\mathrm{tot}} = 
 \begin{bmatrix}
   H_1      	& \tau_1^{+} 	& 0  \\
   \tau_1       	& H_d 			& \tau_2 \\
    0      		& \tau_2^{+} 	& H_2\\
  \end{bmatrix}
$$
	- The size of different matrix is related to the degree-of-freedom of different region	
## Externded Atomistic Green's Function Method
---

**What and How**:

- The extended method is based on the concept of the **Bloch matric**
- It allow us to determine the wavelength and polarizatoin dependence of the phonon transmission
- **Bloch matrix**: describe the **phase change of the eigenmodes** as they propagate from one rincipal layer to another and is associated with the translational symmetry of the leads. 



- Lack of knowledge of phonon _transmission coefficients_ between specific modes on each side of the interface and how the coefficients are affected by **atomic scale structure**.
- Precise transmission and reflection processes that lead to thermal resistance and how they depend on phonon frequency as well as incident angle. 
    + The process can be partly explained with familiar concepts such as **conservation of transverse momentum**.
- Mode-resolved formalism of the AGF
    + transmission coefficient from a specific mode in a material to a specific mode in the other material. 

