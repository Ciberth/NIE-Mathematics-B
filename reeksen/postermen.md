# Reeksen met uitsluitend positieve termen

## Integraalcriterium van Cauchy

Als er voor een reeks met positieve termen $$ \sum a_n $$ een reële functie _f_ bestaat zodat:
- f **continu en dalend** is over $$ [m, +\infty[ $$ 
- $$ f(n) = a_n $$
dan geldt:

- $$ \int_m^\infty f(x)dx \in \mathbb{R} \implies \sum a_n $$ is convergent 
- $$ \int_m^\infty f(x)dx = \infty \implies \sum a_n $$ divergent naar $$ \infty $$ 


## Vergelijkingscriterium 1

Zijn $$ \sum a_n $$ en $$ \sum b_n $$ twee reeksen met positieve termen waarvoor $$ a_n \leq b_n $$ (met a de minorante reeks en b de majorante) dan geldt:

$$ \sum b_n $$ is convergent $$ \implies \sum a_n $$ is convergent $$

en

$$ \sum a_n $$ is divergent $$ \implies \sum b_n $$ is divergent $$

## Vergelijkingscriterium 2

Zijn er twee reeksen $$ \sum a_n $$ en $$ \sum b_n $$ en is de $$ \lim\limits_{n \to +\infty} \frac{a_n}{b_n}$$ noch nul noch oneindig dan zijn de reeksen samen convergent of divergent. Wat de een doet, doet de andere ook.


## Convergentiecriterium van d'Alembert

Bereken de volgende limiet: $$ \lim\limits_{n \to +\infty} \frac{a_{n+1}}{a_n} $$ 
- Is deze limiet **kleiner dan 1** dan is de reeks **convergent**. 
- Is deze limiet **groter dan 1** dan is de reeks **divergent**.
- Is deze limiet **gelijk aan 1** dan hebben we **geen besluit**.


## Convergentiecriterium van Cauchy

Bereken de volgende limiet: $$ \lim\limits_{n \to +\infty} \sqrt[n]{a_n} $$ 
- Is deze limiet **kleiner dan 1** dan is de reeks **convergent**. 
- Is deze limiet **groter dan 1** dan is de reeks **divergent**.
- Is deze limiet **gelijk aan 1** dan hebben we **geen besluit**.
