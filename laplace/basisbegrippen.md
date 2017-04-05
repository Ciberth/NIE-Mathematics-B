# Basisbegrippen Laplace

Dit is een temp test voor latex.

When {% math %}a \ne 0{% endmath %}, there are two solutions to {% math %}(ax^2 + bx + c = 0){% endmath %} and they are {% math %}x = {-b \pm \sqrt{b^2-4ac} \over 2a}.{% endmath %}


When $$a \ne 0$$, there are two solutions to $$(ax^2 + bx + c = 0)$$ and they are $$x = {-b \pm \sqrt{b^2-4ac} \over 2a}.$$



# Definities 

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
                  0  \quad t < -2\\
                  -1 \quad -2 < t < 0 \\
                  1  \quad 0 < t < 1 \\
                  0  \quad 1 < t
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
                  \int_a-\epsilon_{1}^a+\epsilon_{2} \delta(t-a) dt = 1 \quad \forall \epsilon_{1}, \epsilon{2} > 0 
                \end{array}
              \right.
{% endmath %}

De Dirac deltafunctie kan men beschouwen als een **limiet** van een reeks functies. Merk ook op dat de dirac deltafunctie **geen echte functie** is. 

### Eigenschappen

1. $$ \int_-\infty^+\infty f(t)\delta(t-a) dt = f(a) $$ voor elke functie $$ f(t) $$ continu in de omgeving van a.

2. $$ \frac{\mathrm{d}H(t-a)}{\mathrm{d}t} = \delta(t-a) $$.


## Causale functie

Men noemt een functie $$ f(t) $$ **causaal** indien $$ f(t) = 0,\quadt < 0 $$. Tijdsafhankelijke functies illustreren dit (vandaar ook de keuze t als afhankelijke veranderlijke). 

## Functies van exponentiële orde

Men noemt $$ f(t) $$ van **exponentiële orde** indien er reële constanten M en a bestaan, M > 0 zodat 


$$ \forall t > N : |f(t)| < M e^at $$, of m.a.w $$ |f(t)|exp^-at < M $$

Men zegt dat f(t) dan van exponentiële orde a is indien a het **kleinste** getal is waarvoor dit geldt. 

Wil je dit _praktisch_ onderzoeken dan bereken je een limiet:

Er bestaat een $$ a \in \mathbb{R} $$ zodat $$ \[ \lim{t \to +\infty} \frac{|f(t)|}{e^at} \] \in \mathbb{R} $$. 