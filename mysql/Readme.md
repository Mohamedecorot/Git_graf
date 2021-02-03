#Pour créer une base de données
CREATE DATABASE nom

#Pour choisir l'encodage
CREATE DATABASE nom
DEFAULT CHARACTER SET utf8
DEFAULT COLLATE uft8_general_ci;

#Pour supprimer une base de données
DROP DATABASE nom

Pour créer une table
USE nomdelabase;
CREATE TABLE nomdelatable (
    nomduchamp typeduchamp valeurduchamp NOT NULL,
    nomduchamp typeduchamp valeurduchamp NOT NULL,
    nomduchamp typeduchamp valeurduchamp NOT NULL
)

exemple : nom VARCHAR(255) NOT NULL
