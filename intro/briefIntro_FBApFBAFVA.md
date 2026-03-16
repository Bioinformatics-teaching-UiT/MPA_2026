# Differences / Definition of FBA, pFBA, and FVA

very nice (and correct) summary by chatgpt: :-)

## FBA (Flux Balance Analysis) 

FBA computes a single optimal flux distribution that maximizes (or minimizes) a defined objective function (commonly biomass growth) under steady-state and stoichiometric constraints. It uses linear programming to find one feasible solution that achieves the best objective value. However, multiple alternative flux distributions can often yield the same optimal objective.

## **pFBA (parsimonious Flux Balance Analysis)**

pFBA first performs standard FBA to determine the optimal objective value, then minimizes the total sum of fluxes while keeping that objective fixed. This selects the most “economical” solution, favoring minimal overall enzyme usage. It helps reduce flux variability and yields a more biologically realistic, sparse flux distribution.

## FVA (Flux Variability Analysis)

FVA determines the minimum and maximum possible flux for each reaction while maintaining a specified objective value (often the FBA optimum). Instead of giving one solution, it characterizes the full range of feasible fluxes for every reaction. This reveals alternative pathways and the degree of flexibility or redundancy in the metabolic network.

**Sascha:** Of note, you can also run FVA with a pFBA constraint with cobrapy. They have a parameter just for that. One of the most valuable things cobrapy offers with FVA and is, as far as I know, not available in openCOBRA (for whatever reason).