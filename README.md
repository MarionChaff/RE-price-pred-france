# real-estate-price-prediction-france

ENG:

Real estate price prediction tool based on French data and applied to Saint-Malo (35400, Bretagne) 

Building predictive models to estimate real estate prices based on limited property features provided in the state 'DVF' dataset (https://app.dvf.etalab.gouv.fr/).

Three types of model explored:
- A linear regression using scikit-learn
- A boosted tree using XGBoost
- A simple neural network using TensorFlow/Keras

Models input:
- total surface (feature 'surface_reelle_bati'), in sqm
- number of rooms (feature 'nombre_pieces_principales'), in #
- field surface (feature 'surface_terrain'), in sqm
- position (feature 'longitude', 'latitude')
- housing type (house=1 or flat=0 - feature 'maison'), 1 or 0

Models output:
- total price (feature 'valeur_fonciere'), in kEUR

Notebook content:
- Data import
- Data preprocessing and scaling
- Models building, evaluation and comparison

Note on the dataset: The dataset is sourced from DVF data portal, which is openly accessible and provides information on property transactions including transaction price, surface area, location details, and number of rooms. This dataset does not include detailed property conditions or specific features like electrical/plumbing systems, presence of kitchen/bathroom, floor level, brightness, or necessary repairs.

* * *

FR : 

Outil de prédiction des prix de l'immobilier appliqué à Saint-Malo (35400, Bretagne)

Construction de modèles prédictifs pour estimer les prix immobiliers basés sur des caractéristiques (limitées) des biens fournies dans la base de données gouvernementale 'DVF' (https://app.dvf.etalab.gouv.fr/).

Trois types de modèles explorés :
- Une régression linéaire avec scikit-learn
- Un arbre avec XGBoost
- Un réseau de neurones simple avec TensorFlow

Inputs du modèle :
- Surface totale (paramètre 'surface_reelle_bati'), en m²
- Nombre de pièces (paramètre 'nombre_pieces_principales'), en #
- Surface du terrain (paramètre 'surface_terrain'), en m²
- Position (paramètres 'longitude', 'latitude')
- Type de logement (maison=1 ou appartement=0 - paramètre 'maison'), 1 ou 0
  
Output du modèle :
- Prix total (paramètre 'valeur_fonciere'), en kEUR

Contenu du notebook :
- Import des données
- Preprocessing et scaling des données
- Construction, évaluation et comparaison des modèles

Remarques sur le jeu de données : il est issu du portail de données DVF, qui est librement accessible et fournit des informations sur les transactions immobilières incluant le prix de transaction, la surface, les détails de localisation et le nombre de pièces. Il n'inclut pas les conditions détaillées des propriétés ou des caractéristiques spécifiques comme par ex. les systèmes électriques/plomberie, la présence de cuisine/salle de bain, l'étage, la luminosité, les réparations nécessaires, etc.
