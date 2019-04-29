# Découvrez pourquoi Elixir sera votre prochain langage !
**Hands-on Labs**  
Dans cette [session pratique](https://cfp.devoxx.fr/2019/talk/AHP-9443/Decouvrez_pourquoi_Elixir_sera_votre_prochain_langage!), nous avons découvert le langage de programmation fonctionnelle [_Elixir_](https://elixir-lang.org/) et son potentiel prometteur due à la machine virtuelle _BEAM_ et son environnement d'exécution distribué et parallélisé. Nous avons expérimenté avec la syntaxe de ce langage via sa console interactive _iex_ et un example d'une application de Chat avec sa framework Web [_Phoenix_](https://phoenixframework.org/).


# Créer facilement des microservices (ou cloud native java) avec Eclipse MicroProfile
**University**  
[Session](https://cfp.devoxx.fr/2019/talk/LGU-0798/Creer_facilement_des_microservices__(ou_cloud_native_java)_avec_Eclipse_MicroProfile) de live coding où le projet [_Eclipse Microprofile_](https://microprofile.io/) a était présenté comme alternative viable de Spring Boot. Les transparents sont accessibles sous ce [lien](https://speakerdeck.com/lbenoit/creer-facilement-des-microservices-ou-cloud-native-java-avec-eclipse-microprofile?slide=107). Eclipse Microprofile peut être vue comme un ensemble de spécifications du standard J2EE post J2EE 8 visant à standardiser la création d'applications Java Microservice et Cloud Native. Cette spécification a était initiée en 2016 avec la version 1.0 et s'est limitée au départ aux standards CDI 1.2, JAX-RS 2.0 et JSON-P 1.0 pour finir par englober une panoplie de spécifications dans sa version 2.2. Cette dernière finira par contenir les aspects authentification, traçabilité et fault tolerance. La présentation s'est terminée avec les perspectives futures qui consistent à ajouter les Stream réactifs et GraphQL voir être compatible avec Quarkus.
Ce [lien](https://github.com/microprofile-extensions) contient une liste exhaustive et à jour des extensions pour activer les différentes fonctionnalités du Microprofile.

# Quarkus: du live reload à la compilation native
**Tools-in-Action**  
Après une brève présentation de [_Quarkus_](https://quarkus.io/), cette [session](https://cfp.devoxx.fr/2019/talk/HRS-0291/Quarkus:_du_live_reload_a_la_compilation_native) a enchaîné sur un example pratique qui montre l'utilisation d'un fichier de configuration unifié et le gain en taille des livrables et en performance dans les temps de démarrage avec l'approche AoT (Ahead of Time) en coopération avec la [_GraalVM_](https://www.graalvm.org/).

# Micronaut, le framework JVM ultra-light du futur
**Tools-in-Action**  
[_Micronaut_](https://micronaut.io/) est une Framework très récente (apparue en Août 2018) basée sur la JVM. Micronaut se présente comme étant une synthèse des avantages des autres frameworks JVM (Spring, Grails et Spring Boot)

![alt text](./images/micronaut-advantages.png "Micronaut Advantages")

et d'autre part en évitant leur limitations côté conception.

![alt text](./images/micronaut-other-limitations.png "Limitations that Micronaut tried to avoid")

Micronaut se base sur la technique de la compilation anticipée AoT (Ahead of Time) et évite l'usage du mécanisme de la Reflection.

![alt text](./images/micronaut-how-it-works.png "Micronaut: How does it work")

La [présentation](https://cfp.devoxx.fr/2019/talk/WPM-6585/Micronaut,_le_framework_JVM_ultra-light_du_futur) a montré un [example](https://github.com/orevial/twitter-demo-micronaut-kotlin) de chargement de flux Twitter en Kotlin.

# Utiliser les flux réactifs c'est bien, les tester et les debugger c'est mieux !
**Tools-in-Action**  
Cette [présentation](https://cfp.devoxx.fr/2019/talk/XAF-7489/Utiliser_les_flux_reactifs_c'est_bien,_les_tester_et_les_debugger_c'est_mieux_!) a pour but de montrer les difficultés qu'on rencontre lors du teste unitaire d'un code Reactif, en particulier avec les Frameworks [_RxJava_](https://github.com/ReactiveX/RxJava) et [_Reactor_](https://projectreactor.io/). La difficulté vient du fait qu'un code adoptant le paradigme Reactif est multi-threaded donc non déterministe (l'ordre des éléments dans le flux n'est pas nécessairement respecté) et souvent asynchrone. Pour le cas asynchrone, il faut utiliser des Scheduler pour simuler un délais afin d'intercepter la réponse différée. Il y'a aussi des cas où on doit faire attention au volume de la réponse ce qui demande l'utilisation de la technique du _Polling_. Les flux réactifs sont réputés avoir des stack trace cryptiques et difficiles à lire, mais Reactor possède l'avantage d'avoir des sorties plus lisibles. En conclusion, tester des flux réactifs est délicat et demande un effort à part.
