# La Keynote de Devoxx France
**Keynote**  
Présentation de différentes statistiques (nombre de participants, taux de visualisation sur Youtube, logistique), dans une mise en scène drôle, qui sont en globalité positives et montrent le succès de l'événement Devoxx France.

# Le Bonheur au travail : au delà du bullshit.
**Keynote**  
Dans cette [intervention](https://cfp.devoxx.fr/2019/talk/ZGF-7420/Le_Bonheur_au_travail_:_au_dela_du_bullshit.), l'ingénieur et philosophe Christian Fauré, nous expose le côté nuisible et caché d'un environnement de travail vidé de tout sens de valeur ajoutée. Il nous introduit la notion de la _Prolitarisation_ de l'individu qui consiste à le priver du savoir et le transformer en un automate exécutant une tâche monotone semblable à la situation de la classe ouvrière à la veille de la Révolution Industrielle. Il attire notre attention sur les dangers latents que représente l'utilisation excessive des Frameworks informatiques qui visent à améliorer la productivité, vu la nature hautement compétitive du marché, mais qui finissent par nous rendre des esclaves car elles nous éloignent des principes fondamentaux sous jacents (donc du savoir créatif) et limitent notre apport à un savoir superficiel et éphémère. Le bonheur ne vient pas de l'emploie ou du poste occupé, mais de la valeur du Travail qui induit un sentiment de satisfaction venu de l'oeuvre et la quête du savoir et du sens qui sont, enfin du compte, l'essence même de notre éxistence.

# La bienveillance en entreprise
**Keynote**  
Sous le même thème du bonheur au travail, l'ancien commandant de la Marine Nationale Olivier Lajous, enchaîne avec un [discours](https://cfp.devoxx.fr/2019/talk/YMT-2000/La_bienveillance_en_entreprise) qui porte sur la relation avec l'autre dans le milieu du travail. Malgré l'aspect non individuel que relève l'idée d'un group où il y'a la bienveillance, son intervention se base sur le principe que pour être en paix avec les autres, il faut commencer par soi-même. Par conséquence, un groupe où il y'a un conflit entre ses membres accuse un problème interne au niveau individuel. L'intervenant a employé la [Parabole des Porcs-épics](https://www.schopenhauer.fr/fragments/porcs-epics.html) du philosophe Allemand Schopenhauer pour nous expliquer l'importance d'adopter une distance adéquate avec l'autre pour éviter les conflits et pour trouver un compromis pour la cohérence de l'équipe. Il invoque aussi les _4 Accords Toltèques_ (parole impeccable, ne pas prendre les choses d'une manière personnelle, faire de son mieux, ne pas faire de suppositions) comme une philosophie de conduite personnelle pour atteindre la paix interne et par conséquence l'harmonie avec les autres.

# PostgreSQL c'est le nouveau NoSQL
**Conférence**  
Selon le site [db-engines](https://db-engines.com/en/systems), il existe quelque 330 systèmes de base de données de tout types (relationnel ou NoSQL). PostgreSQL a fait l'objet de cette [conférence](https://cfp.devoxx.fr/2019/talk/DRV-0739/PostgreSQL_c'est_le_nouveau_NoSQL) qui avait pour objectif de nous montrer comment ce système de base de données relationnel est inscrit dans la même tendance générale (appelée _NewSQL_) qui consiste à adopter le _Multimodel_ c'est à dire avoir des fonctionnalités NoSQL comme le schema non rigide ou les données documents. Pour commencer, le conférencier à expliqué les concepts NoSQL qui manquent dans les bases relationnelles.

![alt text](./images/pgsql-lacks-nosql.png "What RDBMS lacked")

Ensuite, la présentation a continué avec les fonctionnalités dans PostgreSQL qui visent à mettre en place ces concepts qu'on trouve dans les base NoSQL, à savoir:  
- _Schemaless_: les colonnes indexées du type JSON et JSONB qui portent les types et qui sont indexées.
- _Scalability/Replication, Failure Ready_: la fonctionnalité du _Sharding_ qui assure la réplication et la création des partitions des tables, la réplication peut être physique (copie source destination) ou logique (par stream d'écriture). En outre, PostgreSQL supporte des requêtes distribuées et parallèles.
- _Multimodel_: l'utilisation des _Foreign Data Wrappers_ qui permettent de manipuler des données en provenance d'autres sources NoSQL. Sans oublier les _Temporal Queries_ qui rapprochent PostgreSQL des bases Time Series comme [_Prometheus_](https://prometheus.io/).

Enfin, une démonstration du nouveau <i>Driver JDBC Reactif R2DBC</i> pour montrer comment il nous permet de gérer d'une manière asynchrone et robuste notre connexion.

# Retour aux sources de l'authentification et ce qui va changer en Septembre 2019 pour nos achats
**Conférence**  
Cette [conférence](https://cfp.devoxx.fr/2019/talk/MIT-3734/Retour_aux_sources_de_l'authentification_et_ce_qui_va_changer_en_Septembre_2019_pour_nos_achats) a commencé par relater l'histoire des mécanismes d'authentification (Basic, RFC-2617, stockage dans la base de données, les fichiers apache .htpasswd et .htaccess) pour finir avec la technique actuelle du hashage, Salting et le Work Factor avec des algorithmes comme Argon2, scrypt ou bcrypt.


# Event loop et asynchronisme en JavaScript
**Quickie**  

# Introduction to Face Processing with Computer Vision
**Conférence**  

# Cats, Qubits, and Clouds: The Quantum Future
**Conférence**  

# La gestion de l'authentification et de l'autorisation dans une architecture microservices ? Pas de soucis !
**Conférence**  

# Hexagonal at Scale, où l'art de découper et organiser ses services
**Conférence**  

# S'il te plait... dessine moi un vrai test d'intégration
**Tools-in-Action**  

# Améliorez la performance et l'UX de vos app avec React Suspense
**Tools-in-Action**  
