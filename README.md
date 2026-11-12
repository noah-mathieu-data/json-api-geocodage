# json-api-geocodage

Cours de la semaine 9 de ma formation Data Analyst à la Wild Code School. J'ai appris à lire du JSON, à interroger une API et à placer des adresses sur une carte.

Tout le travail est dans `notebooks/quete_json_api.ipynb`. Les fichiers de départ et le résultat sont dans `data/`.

## Les trois challenges

D'abord j'ai mis à plat un JSON à trois étages avec des villes de Sicile et leurs restaurants. Syracuse a la meilleure note moyenne avec 4,47.

Ensuite j'ai envoyé cinq adresses à l'API Adresse du gouvernement. Quatre ont été trouvées. Pour « Grand Place, Lille » l'API m'a répondu « Place de Gand » avec un score de 0,57. Elle ne prévient jamais quand elle se trompe. Depuis je compare toujours ce que j'ai demandé avec ce qu'on me répond.

Enfin j'ai trouvé la position de quatre restaurants de Catane avec Nominatim et je les ai placés sur une carte. Les coordonnées sont gardées dans `data/restaurants_geocodes.csv` pour ne pas redemander au service à chaque fois.

## Ce qui m'a bloqué

La carte ne s'affichait pas dans VS Code. Je l'ai ouverte dans Jupyter dans le navigateur et là elle marchait.

## Pour le relancer

```bash
python -m venv .venv
source .venv/Scripts/activate
pip install -r requirements.txt
```

Noah Mathieu · [LinkedIn](https://www.linkedin.com/in/noah-mathieu-data)