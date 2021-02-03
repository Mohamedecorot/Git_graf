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