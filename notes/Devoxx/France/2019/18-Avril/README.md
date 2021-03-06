# Jeudi 18 Avril, Devoxx France 2019
**Agenda**  
[La Keynote de Devoxx France](#la-keynote-de-devoxx-france)  
[Le Bonheur au travail : au delà du bullshit.](#le-bonheur-au-travail--au-delà-du-bullshit)  
[La bienveillance en entreprise](#la-bienveillance-en-entreprise)  
[PostgreSQL c'est le nouveau NoSQL](#postgresql-cest-le-nouveau-nosql)  
[Retour aux sources de l'authentification et ce qui va changer en Septembre 2019 pour nos achats](#retour-aux-sources-de-lauthentification-et-ce-qui-va-changer-en-septembre-2019-pour-nos-achats)  
[Event loop et asynchronisme en JavaScript](#event-loop-et-asynchronisme-en-javascript)  
[Introduction to Face Processing with Computer Vision](#introduction-to-face-processing-with-computer-vision)  
[Cats, Qubits, and Clouds: The Quantum Future](#cats-qubits-and-clouds-the-quantum-future)  
[La gestion de l'authentification et de l'autorisation dans une architecture microservices ? Pas de soucis !](#la-gestion-de-lauthentification-et-de-lautorisation-dans-une-architecture-microservices--pas-de-soucis-)  
[Hexagonal at Scale, où l'art de découper et organiser ses services](#hexagonal-at-scale-où-lart-de-découper-et-organiser-ses-services)  
[S'il te plait... dessine moi un vrai test d'intégration](#sil-te-plait-dessine-moi-un-vrai-test-dintégration)  
[Améliorez la performance et l'UX de vos app avec React Suspense](#améliorez-la-performance-et-lux-de-vos-app-avec-react-suspense)  

## La Keynote de Devoxx France
**Keynote**  
Présentation de différentes statistiques (nombre de participants, taux de visualisation sur Youtube, logistique), dans une mise en scène drôle, qui sont globalement positives et montrent le succès de l'événement Devoxx France.

**[:arrow_double_up: Agenda](#jeudi-18-avril-devoxx-france-2019)**

## Le Bonheur au travail : au delà du bullshit.
**Keynote**  
Dans cette [intervention](https://cfp.devoxx.fr/2019/talk/ZGF-7420/Le_Bonheur_au_travail_:_au_dela_du_bullshit.), l'ingénieur et philosophe Christian Fauré, nous expose le côté nuisible et caché d'un environnement de travail vide de tout sens de valeur ajoutée. Il nous introduit la notion de la _Prolitarisation_ de l'individu qui consiste à le priver du savoir et le transformer en un automate exécutant une tâche monotone semblable à la situation de la classe ouvrière à la veille de la Révolution Industrielle. Il attire notre attention sur les dangers latents que représente l'utilisation excessive des Frameworks informatiques qui visent à améliorer la productivité, vu la nature hautement compétitive du marché, mais qui finissent par nous rendre des esclaves car elles nous éloignent des principes fondamentaux sous jacents (donc du savoir créatif) et limitent notre apport à un savoir superficiel et éphémère. Le bonheur ne vient pas de l'emploie ou du poste occupé, mais de la valeur du Travail qui induit un sentiment de satisfaction venu de l'oeuvre et la quête du savoir et du sens qui sont, enfin du compte, l'essence même de notre existence.

**[:arrow_double_up: Agenda](#jeudi-18-avril-devoxx-france-2019)**

## La bienveillance en entreprise
**Keynote**  
Sous le même thème du bonheur au travail, l'ancien commandant de la Marine Nationale Olivier Lajous, enchaîne avec un [discours](https://cfp.devoxx.fr/2019/talk/YMT-2000/La_bienveillance_en_entreprise) qui porte sur la relation avec l'autre dans le milieu professionnel. Malgré l'aspect non individuel que relève l'idée d'un groupe où il y'a la bienveillance, son intervention se base sur le principe suivant: pour être en paix avec les autres, il faut commencer par se réconcilier avec soi-même. Par conséquence, un groupe où il y'a un conflit entre ses membres accuse un problème interne au niveau individuel. L'intervenant a employé la [Parabole des Porcs-épics](https://www.schopenhauer.fr/fragments/porcs-epics.html) du philosophe Allemand Schopenhauer pour nous expliquer l'importance d'adopter une distance adéquate avec l'autre pour éviter les conflits et pour trouver un compromis pour la cohérence de l'équipe. Il invoque aussi les _4 Accords Toltèques_ (parole impeccable, ne pas prendre les choses d'une manière personnelle, faire de son mieux, ne pas faire de suppositions) comme une philosophie de conduite personnelle pour atteindre la paix interne et par conséquence l'harmonie avec les autres.

**[:arrow_double_up: Agenda](#jeudi-18-avril-devoxx-france-2019)**

## PostgreSQL c'est le nouveau NoSQL
**Conférence**  
Selon le site [db-engines](https://db-engines.com/en/systems), il existe quelque 330 systèmes de base de données de tout types (relationnel ou NoSQL). PostgreSQL a fait l'objet de cette [conférence](https://cfp.devoxx.fr/2019/talk/DRV-0739/PostgreSQL_c'est_le_nouveau_NoSQL) qui avait pour objectif de nous montrer comment ce système de base de données relationnel est inscrit dans la même tendance générale (appelée _NewSQL_) qui consiste à adopter le _Multimodel_ c'est à dire avoir des fonctionnalités NoSQL comme le schema non rigide ou les données documents. Pour commencer, le conférencier à expliqué les concepts NoSQL qui manquent dans les bases relationnelles.

![alt text](./images/pgsql-lacks-nosql.png "What RDBMS lacked")

Ensuite, la présentation a continué avec les fonctionnalités dans PostgreSQL qui visent à mettre en place ces concepts qu'on trouve dans les base NoSQL, à savoir:  
- _Schemaless_: les colonnes du type JSON et JSONB qui portent les types et qui sont indexées.
- _Scalability/Replication, Failure Ready_: la fonctionnalité du _Sharding_ qui assure la réplication et la création des partitions des tables, la réplication peut être physique (copie source destination) ou logique (par stream d'écriture). En outre, PostgreSQL supporte des requêtes distribuées et parallèles.
- _Multimodel_: l'utilisation des _Foreign Data Wrappers_ qui permettent de manipuler des données en provenance d'autres sources NoSQL. Sans oublier les _Temporal Queries_ qui rapprochent PostgreSQL des bases Time Series comme [_Prometheus_](https://prometheus.io/).

Enfin, une démonstration du nouveau [_Reactive JDBC Driver R2DBC_](https://r2dbc.io/) pour montrer comment il nous permet de gérer d'une manière asynchrone et robuste notre connexion.

**[:arrow_double_up: Agenda](#jeudi-18-avril-devoxx-france-2019)**

## Retour aux sources de l'authentification et ce qui va changer en Septembre 2019 pour nos achats
**Conférence**  
Cette [conférence](https://cfp.devoxx.fr/2019/talk/MIT-3734/Retour_aux_sources_de_l'authentification_et_ce_qui_va_changer_en_Septembre_2019_pour_nos_achats) a commencé par relater l'histoire des mécanismes d'authentification ([Basic ou RFC-2617](https://www.ietf.org/rfc/rfc2617.txt), stockage dans la base de données, les fichiers Apache [.htpasswd](https://httpd.apache.org/docs/2.4/programs/htpasswd.html) et [.htaccess](https://httpd.apache.org/docs/2.4/howto/htaccess.html)) pour finir avec la technique actuelle du _hashage_, qui se base sur les ingrédients suivants:
- Strong: le mot de passe doit être suffisamment long et contient un maximum de diversité de symbole, donc, imprévisible.
- Adaptative: il fonctionne indépendamment de l'algorithme de chiffrage.
- Salted: l'utilisation d'un _salt_ qui est une entrée aléatoire ajoutée à l'algorithme de hashage afin de varier le résultat qui est le mot de passe chiffré, ça permet d'éviter toute redondance si un mot de passe est choisi plus qu'une fois.
- des algorithmes de hashage robustes comme [Argon2](https://en.wikipedia.org/wiki/Argon2), [scrypt](https://en.wikipedia.org/wiki/Scrypt) ou [bcrypt](https://en.wikipedia.org/wiki/Bcrypt).
 
Le bon choix de ces facteurs va permettre d'augmenter l'effort nécessaire (_Work Factor_) pour déduire le mot de passe à partir de sa transformation.  
Afin d'enforcer la robustesse du choix des mots de passe au niveau application, la conférence suggère d'utiliser des outils de test des mots de passes comme la librairie [zxcvbn](https://github.com/dropbox/zxcvbn) de DropBox ou l'API [HaveIBeenPawned](https://haveibeenpwned.com/API/v2) qui permet de vérifier si un mot de passe a était compromis ou non (au moins selon la base de données sur laquelle se base l'API).

Ci-dessous un résumé sous forme de checklist sur les critères de robustesse d'un système d'authentification.

![alt text](./images/password-authentication-checklist.png "Authentication Strength Checklist")

Dans le cadre actuel des API et des architectures microservices, des protocoles d'authentification sont apparus notamment [_OpenIDConnect_](https://openid.net/connect/) et il est fortement recommandé d'utiliser des OpenID Providers certifiés comme [Auth0](https://auth0.com/), [keycloack](https://www.keycloak.org/) ou [France connect](https://franceconnect.gouv.fr/).

L'authentification est renforcée par un schéma dit _Double Factor Authentication_ ou _2FA_ qui consiste à ajouter un facteur de vérification de l'identité en plus du mot de passe et ce pour les opérations critiques comme le paiement en ligne. Un example simple est celui des codes envoyés par SMS suite à l'authentification afin de compléter la démarche sécurisée. Le deuxième facteur est associé d'une manière unique et sécurisée à l'utilisateur et peut être de nature:
- biométrique: empreinte digitale, reconnaissance faciale
- matériel: carte SIM, badge RSA, les certificats (préconisé par l'ANSSI)
- géographique: empêcher une connexion d'un endroit différent à une courte période après la première
- comportementale: identifier les habitudes de l'utilisateur lors de sa connexion pour bloquer les sessions volées

Concernant la date du Décembre 2019, une directive de la DSP2 (Directive pour les Services de Paiement) va rendre obligatoire le schéma 2FA pour sécuriser les opérations de paiement.

Pour les perspectives futures des standards d'authentification, on peut mentionner:
- _Universal 2nd Factor_ ou [_U2F_](https://en.wikipedia.org/wiki/Universal_2nd_Factor) qui vise à standardiser une forme d'authentification renforcée basée sur des supports matériels comme les clés USB
- le projet [_FIDO2_](https://en.wikipedia.org/wiki/FIDO2_Project)
- [_WebAuthn_](https://webauthn.io/) un standard W3C

**[:arrow_double_up: Agenda](#jeudi-18-avril-devoxx-france-2019)**

## Event loop et asynchronisme en JavaScript
**Quickie**  
Cette brève [présentation](https://cfp.devoxx.fr/2019/talk/YNA-8521/Event_loop_et_asynchronisme_en_JavaScript) nous a montré la gestion en interne de l'asynchronisme en JavaScript dans les navigateurs. En effet, les appels asynchrones sont mis à part dans une Queue spécifique et ne sont exécutés (par l'_Event Loop_ et en mode FIFO) que lorsque la pile des appels est vide.

![alt text](./images/js-async-task-queue.png "Summary on JavaScript Task Queues")

Mais les tasks ne sont pas tous les même, car ils existent des tasks qui sont de nature plus prioritaire comme l'affichage, d'ou l'existence de plusieurs Queue par type.

![alt text](./images/js-async-task-queues-types.png "Summary on JavaScript Task Queues Types")

Les transparents sont disponibles sous ce [lien](https://t.co/TKdWDCUdry).

**[:arrow_double_up: Agenda](#jeudi-18-avril-devoxx-france-2019)**

## Introduction to Face Processing with Computer Vision
**Conférence**  
Une [présentation](https://cfp.devoxx.fr/2019/talk/LQO-4838/Introduction_to_Face_Processing_with_Computer_Vision) sur l'état d'art de la reconnaissance faciale qu'on trouve souvent dans des applications comme FaceBook et SnapShat. La base dans les démarches de traitement d'images est de la considérer comme un _Tensor_ du type (x, y, (R, G, B)) où x et y sont les dimensions de l'image et (R, G, B) les niveaux de couleur. Ils existent deux types d'algorithmes pour la reconnaissance faciale:
- les algorithmes conventionnels basés sur le traitement directe des grandeurs physiques pour aboutir à un modèle (HOG pour Histogram Oriented Gradient) où on calcule un gradient moyen par une zone de 16 pixels pour établir un patron général du visage

![alt text](./images/face-recognition-HOG.png "Conventional Face Recognition Method of Gradient")

- les algorithmes basés sur les réseaux de neurones (Convolutional Neural Networks) et des modèles entraînés au préalable

La bibliothèque [face_recognition](https://github.com/ageitgey/face_recognition) pour Python est bien réputée pour sa simplicité d'utilisation.

**[:arrow_double_up: Agenda](#jeudi-18-avril-devoxx-france-2019)**

## Cats, Qubits, and Clouds: The Quantum Future
**Conférence**  
Cette [conférence](https://cfp.devoxx.fr/2019/talk/KPB-7976/Cats,_Qubits,_and_Clouds:__The_Quantum_Future_) traite le sujet du _Quantum Computing_ et son état d'art. Elle commence par présenter des problèmes liés à notre vie quotidienne et qui sont difficiles à leur obtenir des réponses dans des délais acceptables, par example, le problème d'un parcours optimisé (mieux connu sous le nom du _Problème du Voyageur de Commerce_) sans répétition d'un groupe de villes par un avion, nos moyens actuels de résolution passent 25 minutes pour 10 villes alors que la durée va monter en exponentiel en 27 ans pour 16 villes. En plus, il y'a l'example de l'industrie pharmaceutique où trouver des composés chimiques pour un nouveau médicament demande de calculer un très grand nombre de paramètres liés à la taille de la molécule. Aborder ce problème avec l'approche classique des ordinateurs numériques et en utilisant des approximations ne permet pas de donner des résultats précis et on se trouve avec des erreurs non négligeables.  
Vers la fin des années 80, certains physiciens ont fait le lien entre la théorie de l'information et les propriétés du monde de l'infiniment petit. En effet, la théorie Quantique attribut les propriétés de _Superposition_ et d'intrication ou _Entanglement_ aux systèmes atomiques. Ainsi, un support d'information à l'échelle quantique peut, grace aux propriétés mentionnées auparavant, présenter un avantage sur les ordinateurs classiques:
- Superposition: on peut définir un _Qbit_ qui se trouve dans une superposition de 0 et 1 au contraire d'un bit classique qui est soit 1 soit 0. Mais après la mesure, un Qbit retrouve un état final classique. Cette propriété nous permet de stocker des résultats intermédiaires de calcul.
- Entanglement: un système de plusieurs Qbit peut être mis en état d'intrication où l'état de l'ensemble est lié à l'état de chaque Qbit individuel. Pour un calcul quantique, sa permet de manipuler un grand nombre de possibilités à travers un nombre limité de Qbit en état de superposition.

De ce fait, les algorithmes quantiques possèdent un grand avantage en temps et en resources sur les ordinateurs classiques qui peut être illustré par l'example du [Quantum Card Test](http://research.ibm.com/ibm-q/quantum-card-test/). Dans cette démo, un algorithme classique passe par au plus _O(N)_ itérations alors qu'un algorithme quantique (dans ce cas l'[algorithme de Grover](https://en.wikipedia.org/wiki/Grover%27s_algorithm)) fait au plus _O(sqrt(N))_ tentatives.  
Concernant l'état d'art actuel, les algorithmes et le formalisme nécessaire pour la théorie du Quantum Computing voir aussi l'architecture d'un ordinateur quantique sont disponibles alors que le support matériel n'est pas encore prêt. En effet, mettre en place un système de calcul quantique nécessite de conserver un grand nombre de Qbit en état d'intrication ce qui nécessite de les isoler de l'environnement extérieur pour éviter le phénomène de _Decoherence_. Ce qui explique le nombre limité des Qbit dans les ordinateurs les plus aboutis (20 pour IBM Q).

![alt text](./images/IBM-Q.png "IBM Quantum Computer")

Actuellement, les chercheurs ont dépassé l'étape de l'établissement des fondements mais n'ont pas atteint l'étape de la supériorité quantique ou _Quantum Advantage_ où un ordinateur quantique dépasse un ordinateur classique dans un cas de problème réel.

![alt text](./images/quantum-phases.png "Quantum Computing Phases")

Il faut noter aussi que les ordinateurs IBM quantiques sont accessibles via le [_Cloud_](https://www.research.ibm.com/ibm-q/) et une bibliothèque, [_Qiskit_](https://qiskit.org/), en Python est disponible pour écrire des algorithmes quantiques.

![alt text](./images/quantum-future-evolution.png "Quantum Computing Future Perspectives")

**[:arrow_double_up: Agenda](#jeudi-18-avril-devoxx-france-2019)**

## La gestion de l'authentification et de l'autorisation dans une architecture microservices ? Pas de soucis !
**Conférence**  
[Partage d'expérience](https://cfp.devoxx.fr/2019/talk/JOT-3424/La_gestion_de_l'authentification_et_de_l'autorisation_dans_une_architecture_microservices_%3F_Pas_de_soucis_!) sur un cas de projet réel où il y'a eu besoin de mettre en place un mécanisme d'Authentification et d'Autorisation pour une architecture microservice.  
L'architecture cible pour être sécurisée est illustrée ci-dessous

![alt text](./images/microservice-initial-architecture.png "Overview of the Microservice Architecture")

Pour le choix d'un fournisseur de service d'authentification, l'équipe a écarté une solution "fait maison" car c'est compliqué de cerner tout les détails de la sécurité, et ils ont opté pour le fournisseur KeyCloack.

![alt text](./images/microservice-security-requirements.png "Requirements for the Microservice Security")

Le protocole pour la sécurité sera OpenIDConnect avec le fournisseur KeyCloack.

![alt text](./images/microservice-security-choice.png "Choices for the Microservice Security")

![alt text](./images/microservice-security-tokens.png "Microservice Security and Tokens")

![alt text](./images/microservice-security-sessions.png "Microservice Security and Session Management")

![alt text](./images/microservice-security-groups.png "Security Groups Management")

![alt text](./images/microservice-security-authorization.png "Authorization Management for the Microservice Security")

![alt text](./images/microservice-security-final.png "Final Architecture for the Microservice Security")

![alt text](./images/microservice-security-conclusions.png "Conclusions on Security on Microservices")

Le code source et les slides sont disponibles dans [GitHub](https://github.com/ImFlog/microservices-security).

**[:arrow_double_up: Agenda](#jeudi-18-avril-devoxx-france-2019)**

## Hexagonal at Scale, où l'art de découper et organiser ses services
**Conférence**  
Cette [conférence](https://cfp.devoxx.fr/2019/talk/GDA-0693/Hexagonal_at_Scale,_ou_l'art_de_decouper_et_organiser_ses_services) a fini par énoncer un nouveau principe pour les architectures microservice et le DDD qui est le _Hexagonal at Scale_ qui semble être une conclusion logique après une longue introduction au DDD. En effet, le talon d'Achille d'une architecture microservice typique réside dans son découpage en domaines distincts d'où l'intérêt du DDD. La manière la plus évidente pour découper le monolithe est d'utiliser un découpage par contexte métier (Paiement, Discount) ce qui peut engendrer des effets collatéraux comme une duplication des entités qui vont évoluer d'une manière indépendante (AdresseFacturation, AddresseLivraison). Le découpage dans ce cas va se baser sur une spécification métier non ambiguë et un effort de groupe (_Event Storming_). Étant donnée une délimitation en domaines pour un microservice, plusieurs critères déterminent son succès comme la possibilité de laisser chaque domaine évoluer indépendamment avec sa propre technologie, une forte cohésion avec un faible couplage et une simplicité de déploiement.  
L'architecture hexagonale est une approche pour assurer la cohésion pour un microservice et est appliquée ponctuellement. Elle est centrée sur le concept du _Domain_ et ses interfaces connues sous le nom de _Port_ et _Adapter_. L'intervenant a remarqué que le même motif peut se répéter au niveau global avec un microservice qui fait le role du Domain et les autres périphériques (API Gateway, Proxy, _BFF_) comme microservice Port et Adapter d'où sa "Découverte" du concept de l'_Hexagonal at Scale_. En fin, il y'a eu l'annonce de son nouveau [bouquin](https://www.amazon.fr/Living-Documentation-Cyrille-Martraire/dp/0134689321) sur le DDD.

**[:arrow_double_up: Agenda](#jeudi-18-avril-devoxx-france-2019)**

## S'il te plait... dessine moi un vrai test d'intégration
**Tools-in-Action**  
Cette [session](https://cfp.devoxx.fr/2019/talk/DLJ-1531/S'il_te_plait..._dessine_moi_un_vrai_test_d'integration) a montré un outil fait par l'équipe de Continious Delivery chez OVH, cet outil s'appelle [CDS](https://github.com/ovh/venom) et permet d'exécuter des tests d'intégration. Les intervenants ont commencé par présenter la problématique qui a engendré le développement de cet outil. Les tests d'intégration sont définis comme étant "tester les fonctionnalités d'un système sur l'ensemble des composants via des scénarios utilisateur", ceci dit, le critère global des tests va nécessiter un effort de scripting pour les lancer, dans un ordre bien défini qui reflète le scénario utilisateur, à travers tout le système. En pratique, les auteurs de l'outil se sont trouvé avec un script Shell de plus de 300 lignes difficile à maintenir. L'outil CDS qui ont développé se base sur les principes suivants:
- pas de _boilerplate_ code: zero ligne code à écrire pour spécifier les tests, juste les fichiers de configuration
- multi-protocole: il supporte tout les types de communication inter-composant (Web, mail ...)
- accessible par les interfaces en mode ligne de commande
- intégrable dans les pipelines CI/CD

En pratique, les _Test Suit_ sont spécifiés dans des fichiers .yml qui contiennent une succession de scénarios à exécuter par l'outil [venom](https://github.com/ovh/venom/tree/master/tests) en ligne de commande.

**[:arrow_double_up: Agenda](#jeudi-18-avril-devoxx-france-2019)**

## Améliorez la performance et l'UX de vos app avec React Suspense
**Tools-in-Action**  
[Démonstration](https://cfp.devoxx.fr/2019/talk/EJW-3475/Ameliorez_la_performance_et_l'UX_de_vos_app_avec_React_Suspense) de la nouvelle API React Suspense pour le chargement asynchrone des composants, cette API permet, d'une manière générique, de suspendre l'affichage en attendant qu'une resource (image, video) ou un autre composant soit prêt.  
Le code source qui a servit pour la démo est disponible sous ce [lien](https://github.com/romaindso/devoxx-2019).

**[:arrow_double_up: Agenda](#jeudi-18-avril-devoxx-france-2019)**
