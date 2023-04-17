# VoorbeeldShop_opdr3

Voor deze opdracht hebben we moeten kijken naar de data die de op = op voordeelshop voor ons publiek heeft gesteld.
Het is namelijk essentieel om de klant te begrijpen. Wij kunnen niet als winkel producten aan gaan smeren.
Dit moet op een meer natuurlijke manier, dit kunnen we door verbanden te leggen in de data.

Welke verbanden zijn er?

We hebben collaborative filtering.
  - Er wordt rekening gehouden met gelijken klanten
  - Er wordt gekeken naar wat die klanten hebben gezien/gekocht
 
Bij deze heb ik een simpele functie gemaakt. Heel algemeen.
De meest bekeken producten worden weergegeven. We nemen alle sessies van alle klanten.
In die sessies zitten namelijk de products die ze hebben bekeken. Zo ritsen we de hele database af.
En houden we voor elk gevonden product een teller bij.

En we hebben content filtering
  - Er wordt gekeken naar de eigenschappen van bepaalde producten
  - Er worden verbanden gelegd tussen die producten
  
Bij deze heb ik een geavenceerde aanpak genomen. Het is vrij doorsnee om bij een similair_products alleen te kijken naar de categoriën.
Ik wilde iets specifieker en kwam daarbij bij count vectorization.
Dit houdt in dat er met een cosine similairity, producten met elkaar worden vergeleken.
Zo wordt er een lijst gemaakt van meest overeenkomend naar minst overeenkomend.
