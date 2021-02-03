# Pour créer une base de données
CREATE DATABASE nom

#Pour choisir l'encodage
CREATE DATABASE nom
DEFAULT CHARACTER SET utf8
DEFAULT COLLATE uft8_general_ci;

# Pour supprimer une base de données
DROP DATABASE nom

# Pour créer une table
USE nomdelabase;
CREATE TABLE nomdelatable (
    nomduchamp typeduchamp valeurduchamp NOT NULL,
    nomduchamp typeduchamp valeurduchamp NOT NULL,
    nomduchamp typeduchamp valeurduchamp NOT NULL
)

exemple : nom VARCHAR(255) NOT NULL

# Pour insérer des données dans une table
INSERT INTO nomdelatable
VALUES ("champ1", "champ2" ...);  (si autoincrément on met NULL)

On peut aussi faire (syntaxe alternative (propre a mysql)):
INSERT INTO nomdelatable SET
nomduchamp1="valeur1", nomduchamp2="valeur2";

# Suppression de données

Pour la suppression simple:
DELETE FROM [table] WHERE [condition]
Pour sécurisé la suppression on peut ajouter le nombre de ligne a supprimer en ajoutant par exemple: LIMIT 1

Et pour vider totalement et efficacement une table
TRUNCATE TABLE nomdelatable

# Modification de données

Pour la modification simple:
UPDATE [table] SET champ=valeur, champ=valeur WHERE [conditions]
(Pour sécurisé la modification on peut ajouter le nombre de ligne a supprimer en ajoutant par exemple: LIMIT 1
)

# Lecture de données

Pour la sélection simple:
SELECT champ champ champ FROM [table] WHERE [conditions]

- Si on veut, on peut limiter la sélection avec LIMIT
    Si on précise un seul chiffre après, cela signifie de 0 à ce chiffre
    Si on précise un deux chiffres après, cela signifie du 1er chiffre au 2eme (c'est ainsi qu'on fera la pagination par exemple)

- Si on veut récupérer tous les champs on peut utiliser un joker * :
    SELECT * FROM [table] WHERE [conditions]

- On peut également organiser les données en ajoutant ORDER BY suivi du nom du champ et on peut ajouter DESC pour inverser l'ordre

- On peut également compter le nombre de données avec COUNT(*)

- On peut également renommer un champ en utisant as
Exemple: SELECT COUNT(*) as population FROM utlisateurs
