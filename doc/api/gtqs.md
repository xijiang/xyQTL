### gtqs: genotype quick simulation
```julia
function gtqs(nid, nlc; maf = .2, α = .75, β = 0.75)
```
This function simulate $n_{ID} \times n_{loci}$ matrix of Int8.
It uses a Beta($\alpha$, $\beta$) distrition to sample allele frequencies,
such that they have a U-shaped distribution.
No LD information is considered.

Example:
```julia
gt = QTL.Simu.gtqs(100, 200)
```
