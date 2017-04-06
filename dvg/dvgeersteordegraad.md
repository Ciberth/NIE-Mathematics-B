# DVG van eerste orde en eerste graad

**Notatie:** $$ M(x,y)dx + N(x,y)dy = 0 $$

## Gescheiden veranderlijken

Dit is het geval als je de gelijkheid kan schrijven opdat beide leden geïntegreerd kunnen worden naar respectievelijk 2 verschillende veranderlijken. Concreet a aantal vergelijkingen in functie van x in het linkerlid en b aantal vergelijkingen in functie van y in het rechterlid. 

## Homogene DVG's

Een DVG is homogeen als $$ M(x,y) $$ en $$ N(x,y) $$ homogeen zijn van dezelfde graad. 

## Totale DVG's

Een DVG is **totaal** of **exact** als het eerste lid van de vergelijking een totalle differentiaal is of m.a.w. als er een functie $$ F(x,y) $$ bestaat zodat $$ dF(x,y) = M(x,y) + N(x,y)dy $$

TODO: Bewijs + stelling van Clairaut

**Opmerkingen:** 
- Let op dat DVG naar nul is herleid voor je de voorwaarde van Euler controleert. 
- Als je een totale DVG met een veranderlijke vermenigvuldigt is ze meestal niet meer totaal. 

## Lineaire DVG's

Een DVG is **lineair in** y **en** y' als ze kan geschreven worden in de vorm: $$ y' + yP(x) = Q(x) $$

**Methode:** stel y=uv (of x=uv), de DVG wordt dan:

$$ u'v + v'u + uvP(x) = Q(x) $$ 

Kies vervolgens een functie v zodat de coëfficiënt van u nul wordt: m.a.w. $$ v' + vP(x) = 0 $$

## DVG van Bernoulli

Deze is van het type: $$ y' + yP(x) = y^nQ(x) $$

**Methode:** 
- Deel de vergelijking door $$ y^n $$. 
- Stel $$ z = y^{1-n} $$.
- Zo krijg je een nieuwe vergelijking die lineair is in z en z'.  