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

$$ f(t) $$ kan dan met met behulp van de Heaviside geschreven worden als $$ f(t) = -H(t+2) +2H(t)-H(t-1) $$.