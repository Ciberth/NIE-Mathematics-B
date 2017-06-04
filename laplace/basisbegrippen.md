# Basisbegrippen Laplace

## De Heaviside functie

De heaviside functie (ook wel eenheidsstapfunctie genoemd) wordt $$ \forall a \in \mathbb{R} $$ gedefineerd als:

{% math %}
    H(t-a)=\left\{
                \begin{array}{ll}
                  0 \quad t < a\\
                  1 \quad t > a 
                \end{array}
              \right.
{% endmath %}

Stuksgewijze continue functies worden vaak met behulp van de Heaviside functie gedefineerd. 

Voorbeeld:

{% math %}
    f(t)=\left\{
                \begin{array}{ll}
                  0  \quad \quad t < -2\\
                  -1 \quad -2 < t < 0 \\
                  1  \quad \quad 0 < t < 1 \\
                  0  \quad \quad 1 < t
                \end{array}
              \right.
{% endmath %}

$$ f(t) $$ kan dan met met behulp van de Heaviside geschreven worden als 

$$ f(t) = -H(t+2) +2H(t)-H(t-1) $$.

**Tips & werkwijze:** Voeg altijd een regel toe die zegt dat de functie causaal is (dit is 0 voor t < 0). Redeneer en onthou "min de vorige plus de huidige" (of een variant: min de huidige plus de volgende).


## De Dirac deltafunctie

### Definitie

De Dirac deltafunctie (ook wel eenheidsimpuls genoemd) wordt $$ \forall a \in \mathbb{R} $$ gedefineerd als:

{% math %}
\left\{
                \begin{array}{ll}
                  \delta(t-a)=0 \quad t \neq a\\
                  \int_{a-\epsilon_{1}}^{a+\epsilon_{2}} \delta(t-a) dt = 1 \quad \forall \epsilon_{1}, \epsilon{2} > 0 
                \end{array}
              \right.
{% endmath %}

De Dirac deltafunctie kan men beschouwen als een **limiet** van een reeks functies. Merk ook op dat de dirac deltafunctie **geen echte functie** is. 

### Eigenschappen

1. $$ \int_{-\infty}^{+\infty} f(t)\delta(t-a) dt = f(a) $$ voor elke functie $$ f(t) $$ continu in de omgeving van a.

2. $$ \frac{\mathrm{d}H(t-a)}{\mathrm{d}t} = \delta(t-a) $$.


## Causale functie

Men noemt een functie $$ f(t) $$ **causaal** indien $$ f(t) = 0,\quad t < 0 $$. Tijdsafhankelijke functies illustreren dit (vandaar ook de keuze t als afhankelijke veranderlijke). 

## Functies van exponentiële orde

Men noemt $$ f(t) $$ van **exponentiële orde** indien er reële constanten M en a bestaan, M > 0 zodat 


$$ \forall t > N : |f(t)| < M e^{at} $$, of m.a.w $$ |f(t)|e^{-at} < M $$

Men zegt dat f(t) dan van exponentiële orde a is indien a het **kleinste** getal is waarvoor dit geldt. 

Wil je dit _praktisch_ onderzoeken dan bereken je een limiet:

Er bestaat een $$ a \in \mathbb{R} $$ zodat $$ \lim\limits_{t \to +\infty} \frac{|f(t)|}{e^{at}} \in \mathbb{R} $$. 


# Definitie van de Laplacetransformatie


Is f(t) causaal, dan definieert men de Laplacegetransformeerde van f(t) als de oneigenlijke Riemann-integraal:

$$ \mathscr{L}\{f(t)\}(s) = F(s) = \int_0^{+\infty} f(t)e^{-st} dt , \quad s \in \mathbb{C} $$.

De Laplacegetransformeerde is dus een functie van $$ s \in \mathbb{C} $$ en zet een causale functie in t om naar een functie over de complexe getallen ( $$ = F(s) $$).


TODO bewijs (p5): aantonen dat F(s) bestaat indien de integraal **absoluut** convergeert.


**Opmerking 1:** Uit de definitie blijkt dat het bestaan van $$ \mathscr{L}\{f(t)\}(s) $$ evenwaardig is met het convergeren van de oneigenlijke integraal. Deze integraal hangt af van de causale functie en van de complexe variabele s.

**Opmerking 2:** Uit de definitie volgt ook de **lineariteit** van de Laplacetransformatie.

Het Laplacebeeld bestaat indien f(t) **causaal** is, **stuksgewijs continue** over elk eindig interval ]0,N] en **exponentieel van orde a** voor t > N. 

Merk ook op dat het laplacebeeld enkel gedefineerd is voor causale functies. Impliciet staat de Heaviside functie in t (H(t)) ook na elke functie (=causaal).



