# Cahier des charges - Application de gestion de porcherie moderne

## 1. Vision du projet

L'objectif est de concevoir une application simple, robuste et moderne pour aider les fermiers a gerer une porcherie dans le contexte africain. L'application doit permettre de suivre les animaux, la reproduction, la sante, l'alimentation, les stocks, les ventes et la rentabilite, tout en restant facile a utiliser sur telephone.

L'application vise les petites, moyennes et grandes porcheries qui souhaitent passer d'une gestion papier ou informelle a une gestion numerique fiable.

## 2. Public cible

### Utilisateurs principaux

- Proprietaire de porcherie
- Gerant de ferme
- Employe charge des soins quotidiens
- Veterinaire ou technicien d'elevage
- Comptable ou responsable financier

### Contexte d'utilisation

- Utilisation majoritairement sur smartphone Android
- Connexion internet parfois instable
- Besoin de saisie rapide sur le terrain
- Niveau numerique variable selon les utilisateurs
- Gestion en francais, avec possibilite future d'ajouter des langues locales
- Utilisation de devises locales comme FCFA, CDF, GNF, XOF, XAF ou autre selon le pays

## 3. Objectifs metier

L'application doit permettre de :

- Connaitre le nombre exact d'animaux par categorie
- Suivre l'historique de chaque animal ou lot
- Reduire les pertes par un meilleur suivi sanitaire
- Ameliorer la reproduction et le sevrage
- Controler les depenses alimentaires
- Suivre les stocks d'aliments, medicaments et materiel
- Enregistrer les ventes et calculer la rentabilite
- Produire des rapports simples pour le proprietaire ou les partenaires
- Aider le fermier a prendre de meilleures decisions

## 4. Perimetre de la premiere version

La premiere version doit etre utilisable par un fermier sans complexite excessive. Elle doit se concentrer sur les fonctions essentielles.

### Modules inclus dans la V1

1. Tableau de bord
2. Gestion du cheptel
3. Reproduction
4. Sante animale
5. Alimentation
6. Stocks
7. Ventes et finances simples
8. Taches quotidiennes
9. Rapports de base
10. Gestion des utilisateurs

### Modules reportes a une version future

- Intelligence artificielle pour previsions avancees
- Capteurs connectes et objets IoT
- Paiement mobile integre
- Marketplace d'achat et vente de porcs
- Gestion multi-fermes avancee
- Synchronisation avec cabinet veterinaire externe
- Reconnaissance photo des animaux

## 5. Fonctionnalites detaillees

## 5.1 Tableau de bord

Le tableau de bord doit afficher rapidement :

- Nombre total d'animaux
- Nombre de truies
- Nombre de verrats
- Nombre de porcelets
- Nombre de porcs en engraissement
- Naissances recentes
- Mortalites recentes
- Alertes sanitaires
- Stocks faibles
- Ventes du mois
- Depenses du mois
- Benefice estime

## 5.2 Gestion du cheptel

Chaque animal ou lot doit pouvoir etre enregistre avec :

- Identifiant unique
- Nom ou numero de marquage
- Categorie : truie, verrat, porcelet, engraissement, reforme
- Race ou croisement
- Sexe
- Date de naissance ou date d'entree
- Origine : ne a la ferme, achat, don, transfert
- Poids actuel
- Statut : actif, vendu, mort, reforme
- Emplacement : batiment, loge, parc ou enclos
- Observations

Pour les petites fermes, l'application doit aussi permettre une gestion par lot au lieu d'une fiche individuelle pour chaque animal.

## 5.3 Reproduction

Le module reproduction doit permettre de suivre :

- Detection des chaleurs
- Saillie naturelle
- Insemination artificielle
- Verrat utilise
- Date de saillie ou insemination
- Date probable de mise bas
- Confirmation de gestation
- Mise bas
- Nombre de porcelets nes vivants
- Nombre de mort-nes
- Nombre de porcelets sevrés
- Date de sevrage
- Historique reproductif par truie

L'application doit generer des alertes pour :

- Retour probable en chaleur
- Diagnostic de gestation
- Mise bas approchee
- Sevrage prevu

## 5.4 Sante animale

Le module sante doit inclure :

- Enregistrement des maladies
- Symptomes observes
- Traitements administres
- Medicament utilise
- Dose
- Date de traitement
- Responsable du traitement
- Veterinaire associe
- Vaccinations
- Vermifuges
- Mortalites
- Cause probable de mortalite
- Periode de retrait avant vente si medicament concerne

Des alertes doivent rappeler :

- Vaccins a venir
- Traitements a renouveler
- Animaux sous observation
- Periodes de retrait non terminees

## 5.5 Alimentation

Le module alimentation doit permettre de suivre :

- Types d'aliments disponibles
- Rations par categorie d'animal
- Quantite distribuee par jour
- Consommation par lot
- Cout de l'aliment
- Evolution des stocks d'aliments
- Estimation du cout alimentaire par animal ou par lot

L'application doit aider a identifier :

- Les lots qui consomment beaucoup
- Les periodes de rupture de stock
- Le cout alimentaire total

## 5.6 Stocks

Le module stocks doit gerer :

- Aliments
- Medicaments
- Vaccins
- Produits de nettoyage
- Petit materiel

Chaque article doit avoir :

- Nom
- Categorie
- Quantite disponible
- Unite : kg, sac, litre, dose, boite, piece
- Seuil d'alerte
- Prix d'achat
- Fournisseur
- Date d'entree
- Date d'expiration si applicable

## 5.7 Ventes et finances simples

Le module financier doit enregistrer :

- Ventes de porcs vivants
- Ventes de porcelets
- Ventes de viande si applicable
- Prix de vente
- Client
- Date de vente
- Mode de paiement
- Montant paye
- Reste a payer
- Depenses : aliment, medicament, main-d'oeuvre, transport, entretien

L'application doit afficher :

- Chiffre d'affaires
- Total des depenses
- Marge estimee
- Creances clients
- Rentabilite par lot si possible

## 5.8 Taches quotidiennes

Le module taches doit permettre de planifier et cocher :

- Nourrir les animaux
- Nettoyer les loges
- Verifier l'eau
- Observer les chaleurs
- Administrer un traitement
- Peser un lot
- Controler les stocks
- Preparer une vente

Chaque tache doit avoir :

- Titre
- Date
- Priorite
- Responsable
- Statut : a faire, en cours, termine

## 5.9 Rapports

La V1 doit permettre de generer des rapports simples :

- Rapport du cheptel
- Rapport sanitaire
- Rapport reproduction
- Rapport ventes
- Rapport depenses
- Rapport stocks
- Rapport mensuel global

Les rapports doivent etre exportables en PDF ou imprimables dans une version future proche.

## 6. Exigences non fonctionnelles

## 6.1 Simplicite

L'interface doit etre claire, avec peu de texte inutile, des boutons visibles et des formulaires courts. Les actions courantes doivent etre accessibles en moins de trois clics.

## 6.2 Mobile-first

L'application doit etre concue d'abord pour telephone Android, puis adaptee aux tablettes et ordinateurs.

## 6.3 Mode hors ligne

L'application doit pouvoir fonctionner sans internet pour les actions essentielles :

- Ajouter des animaux
- Enregistrer soins et traitements
- Saisir alimentation
- Enregistrer ventes et depenses
- Consulter les donnees deja chargees

Les donnees doivent se synchroniser quand la connexion revient.

## 6.4 Securite

L'application doit proteger les donnees par :

- Connexion avec mot de passe
- Roles utilisateurs
- Sauvegardes regulieres
- Journal des actions importantes

## 6.5 Performance

L'application doit rester fluide sur des telephones Android d'entree ou milieu de gamme.

## 7. Roles utilisateurs

### Proprietaire

- Acces complet
- Consultation des finances
- Rapports
- Gestion des utilisateurs

### Gerant

- Gestion quotidienne complete
- Cheptel, reproduction, sante, stocks, ventes
- Acces financier limite selon choix du proprietaire

### Employe

- Consultation des taches
- Saisie des soins simples
- Saisie alimentation
- Signalement de probleme

### Veterinaire

- Consultation sanitaire
- Ajout de traitements
- Historique medical

## 8. Donnees principales

Les principales entites de donnees sont :

- Ferme
- Utilisateur
- Animal
- Lot
- Evenement de reproduction
- Mise bas
- Traitement
- Vaccination
- Mortalite
- Aliment
- Stock
- Mouvement de stock
- Vente
- Depense
- Client
- Fournisseur
- Tache
- Rapport

## 9. Parcours utilisateur essentiels

## 9.1 Ajouter un animal

1. L'utilisateur ouvre le module Cheptel
2. Il choisit Ajouter
3. Il saisit les informations essentielles
4. Il enregistre
5. L'animal apparait dans la liste et le tableau de bord est mis a jour

## 9.2 Enregistrer une mise bas

1. L'utilisateur ouvre la fiche de la truie
2. Il selectionne Mise bas
3. Il saisit la date, les porcelets vivants, mort-nes et observations
4. Le systeme cree ou met a jour les porcelets
5. Une alerte de sevrage est programmee

## 9.3 Enregistrer un traitement

1. L'utilisateur ouvre Sante
2. Il choisit animal ou lot
3. Il saisit symptome, medicament, dose et date
4. Le stock de medicament est mis a jour
5. Une alerte de renouvellement ou retrait est creee si necessaire

## 9.4 Enregistrer une vente

1. L'utilisateur ouvre Ventes
2. Il selectionne les animaux vendus
3. Il saisit client, prix et paiement
4. Les animaux passent au statut vendu
5. Le chiffre d'affaires est mis a jour

## 10. Indicateurs cles

L'application doit aider a suivre :

- Taux de mortalite
- Nombre moyen de porcelets par mise bas
- Taux de sevrage
- Cout alimentaire mensuel
- Chiffre d'affaires mensuel
- Marge estimee
- Stock restant en jours
- Nombre d'alertes ouvertes

## 11. Architecture recommandee

Pour une premiere application utilisable :

- Application web mobile-first installable sur telephone
- Interface en francais
- Base de donnees locale avec synchronisation cloud future
- Backend API pour les donnees partagees
- Possibilite d'evolution vers application mobile native

Technologies possibles :

- Frontend : React, Vue ou Angular
- Backend : Node.js, Laravel ou Django
- Base de donnees : PostgreSQL pour serveur, SQLite ou IndexedDB pour le mode hors ligne
- Export : PDF et Excel dans une version suivante

## 12. Priorites de developpement

### Phase 1 - Prototype utilisable

- Tableau de bord
- Cheptel
- Reproduction simple
- Sante simple
- Stocks alimentaires
- Ventes et depenses simples

### Phase 2 - Gestion avancee

- Alertes automatiques
- Rapports PDF
- Mode hors ligne renforce
- Gestion multi-utilisateurs
- Rentabilite par lot

### Phase 3 - Modernisation avancee

- Application mobile native
- Paiement mobile
- Capteurs connectes
- Previsions de production
- Marketplace locale

## 13. Criteres d'acceptation de la V1

La V1 sera consideree comme utilisable si un fermier peut :

- Creer sa ferme
- Ajouter ses animaux ou lots
- Suivre les naissances et sevrages
- Enregistrer maladies et traitements
- Suivre les stocks d'aliments
- Enregistrer ventes et depenses
- Voir un tableau de bord clair
- Obtenir un rapport simple de son activite
- Utiliser les fonctions essentielles sur telephone

## 14. Questions a valider avec le porteur du projet

1. Dans quel pays l'application sera-t-elle d'abord utilisee ?
2. Quelle devise doit etre prioritaire ?
3. Les fermiers gerent-ils surtout les animaux individuellement ou par lots ?
4. Faut-il prevoir une utilisation sans internet des la V1 ?
5. Les utilisateurs seront-ils principalement francophones ?
6. La porcherie cible a-t-elle moins de 50, 50 a 500, ou plus de 500 porcs ?
7. Faut-il gerer plusieurs fermes dans un meme compte ?
8. Les ventes se font-elles surtout au poids, par animal, ou par lot ?
9. Le proprietaire veut-il suivre les performances des employes ?
10. Faut-il prevoir des rapports pour banques, investisseurs ou services veterinaires ?

## 15. Prochaine etape

La prochaine etape consiste a transformer ce cahier des charges en :

1. liste des ecrans de l'application ;
2. parcours utilisateurs detailles ;
3. modele de base de donnees ;
4. prototype visuel ;
5. premiere version fonctionnelle.
