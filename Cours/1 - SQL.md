# SQL

SQL est un langage informatique utilisé pour gérer et interroger des bases de données. C'est un outil puissant pour stocker et récupérer des données. Alors, préparez-vous à devenir un véritable "Ninja de la Base de Données" ! 😎

### **Chapitre 1 : Qu'est-ce que SQL ?**

SQL, ou Structured Query Language, est un langage de programmation qui vous permet de communiquer avec des bases de données. Les bases de données sont comme des entrepôts où vous pouvez stocker toutes sortes d'informations, comme les scores de jeux vidéo, les informations sur les personnages de vos séries préférées, ou même la liste de vos films préférés.

### **Chapitre 2 : Comment créer une base de données**

Pour commencer, vous devez créer une base de données pour stocker vos données. C'est un peu comme créer un cahier où vous écrirez toutes vos informations. Voici comment vous pouvez faire cela avec SQL :

```php
CREATE DATABASE MaBaseDeDonnees;
```

### **Chapitre 3 : Les tables, où vivent les données**

Une base de données est composée de tables, qui sont comme des feuilles dans votre cahier. Chaque table a des colonnes pour organiser les données. Par exemple, si vous avez une table pour les jeux vidéo, vous pourriez avoir des colonnes pour le nom du jeu, le genre, et le score.

```php
CREATE TABLE JeuxVideo (
    NomDuJeu VARCHAR(50),
    Genre VARCHAR(20),
    Score INT
);
```

### **Chapitre 4 : Insérer des données**

Maintenant que vous avez votre base de données et votre table, il est temps d'y ajouter des données. C'est comme écrire les détails de vos jeux vidéo préférés dans votre cahier.

```php
INSERT INTO JeuxVideo (NomDuJeu, Genre, Score)
VALUES ('Minecraft', 'Aventure', 95);

INSERT INTO JeuxVideo (NomDuJeu, Genre, Score)
VALUES ('Fortnite', 'Bataille Royale', 85);
```

**Tips** : La commande **INSERT INTO** permet au choix d’inclure une seule ligne à la base existante ou plusieurs lignes d’un coup.

### **Chapitre 5 : Interrogation de données**

L'une des parties les plus cool de SQL est la possibilité de poser des questions à votre base de données. Voici comment vous pouvez le faire :

```php
SELECT NomDuJeu, Score
FROM JeuxVideo
WHERE Genre = 'Aventure';
```

Cette requête vous donnera les noms des jeux d'aventure et leurs scores correspondants dans votre base de données.

**Tips** : La commande **WHERE** dans une requête SQL permet d’extraire les lignes d’une base de données qui respectent une condition. Cela permet d’obtenir uniquement les informations désirées

### **Chapitre 6 : Mettez à jour vos données**

Parfois, vous devrez peut-être mettre à jour des informations dans votre base de données. Par exemple, si le score de Minecraft augmente, vous pouvez le faire comme ceci :

```php
UPDATE JeuxVideo
SET Score = 97
WHERE NomDuJeu = 'Minecraft';
```

**Tips** : La commande **UPDATE** permet d’effectuer des modifications sur des lignes existantes. Très souvent cette commande est utilisée avec WHERE pour spécifier sur quelles lignes doivent porter la ou les modifications.

### **Chapitre 7 : Supprimer des données**

Si vous avez besoin de retirer un jeu de votre base de données, voici comment le faire :

```php
DELETE FROM JeuxVideo
WHERE NomDuJeu = 'Fortnite';
```

**Tips** : La commande **DELETE** en SQL permet de supprimer des lignes dans une table. En utilisant cette commande associé à WHERE il est possible de sélectionner les lignes concernées qui seront supprimées.

### **Chapitre 8 : Conclusion**

Félicitations, vous êtes maintenant un Ninja de la Base de Données ! Vous savez comment créer, ajouter, interroger, mettre à jour et supprimer des données dans une base de données SQL. Vous pouvez maintenant gérer vos données comme un pro.

N'oubliez pas que SQL est un outil puissant utilisé dans le monde réel pour gérer d'énormes quantités de données. Alors, continuez à explorer et à vous amuser avec SQL ! Si vous avez des questions ou si vous voulez en savoir plus, n'hésitez pas à demander. 🚀