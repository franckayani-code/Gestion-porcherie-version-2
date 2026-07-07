# Ecrans et parcours utilisateurs - Application de gestion de porcherie

## 1. Objectif du document

Ce document transforme le cahier des charges en structure concrete d'application. Il decrit les ecrans, les menus, les actions disponibles et les parcours principaux pour obtenir une application simple a utiliser par les fermiers.

L'approche retenue est mobile-first : chaque ecran doit etre lisible et pratique sur telephone Android.

## 2. Structure generale de navigation

L'application doit proposer une navigation simple avec un menu principal compose de :

1. Tableau de bord
2. Cheptel
3. Reproduction
4. Sante
5. Alimentation
6. Stocks
7. Ventes
8. Depenses
9. Taches
10. Rapports
11. Parametres

Sur telephone, les modules les plus utilises peuvent etre accessibles dans une barre inferieure :

- Accueil
- Cheptel
- Alertes
- Ajouter
- Menu

Le bouton Ajouter doit permettre une saisie rapide : animal, naissance, traitement, aliment distribue, vente, depense ou tache.

## 3. Ecran de demarrage

### Objectif

Permettre a l'utilisateur d'acceder rapidement a sa ferme ou de creer une ferme au premier lancement.

### Elements affiches

- Logo ou nom de l'application
- Champ telephone ou email
- Champ mot de passe
- Bouton Connexion
- Lien Mot de passe oublie
- Bouton Creer une ferme

### Premiere utilisation

Lors de la premiere utilisation, l'utilisateur renseigne :

- Nom de la ferme
- Pays
- Devise
- Nom du proprietaire
- Telephone
- Taille approximative du cheptel
- Mode de gestion prefere : par animal, par lot, ou mixte

## 4. Tableau de bord

### Objectif

Donner une vision rapide de l'etat de la porcherie.

### Informations principales

- Total animaux
- Truies
- Verrats
- Porcelets
- Porcs en engraissement
- Animaux malades ou sous observation
- Naissances recentes
- Mortalites recentes
- Stocks faibles
- Ventes du mois
- Depenses du mois
- Solde estime

### Actions rapides

- Ajouter animal
- Declarer mise bas
- Enregistrer traitement
- Saisir aliment distribue
- Enregistrer vente
- Ajouter depense

### Alertes visibles

- Mise bas proche
- Sevrage prevu
- Vaccin a faire
- Stock faible
- Medicament bientot expire
- Client avec reste a payer

## 5. Module Cheptel

## 5.1 Liste du cheptel

### Objectif

Afficher tous les animaux ou lots de la ferme.

### Filtres

- Tous
- Truies
- Verrats
- Porcelets
- Engraissement
- Vendus
- Morts
- Reformes

### Informations affichees par ligne

- Identifiant ou nom
- Categorie
- Age ou date d'entree
- Poids si disponible
- Statut
- Emplacement

### Actions

- Rechercher un animal
- Filtrer par categorie
- Ajouter animal
- Ajouter lot
- Ouvrir fiche detaillee

## 5.2 Fiche animal

### Objectif

Consulter l'historique complet d'un animal.

### Sections

- Identite
- Etat actuel
- Reproduction si animal reproducteur
- Sante
- Poids
- Alimentation si suivi individuel
- Historique
- Documents ou photos dans une version future

### Actions

- Modifier informations
- Ajouter pesee
- Declarer maladie
- Ajouter traitement
- Programmer vaccin
- Enregistrer vente
- Declarer mortalite
- Changer emplacement

## 5.3 Fiche lot

### Objectif

Gerer plusieurs animaux ensemble, surtout pour les porcelets et l'engraissement.

### Informations

- Nom du lot
- Categorie
- Nombre initial
- Nombre actuel
- Date de creation
- Poids moyen
- Emplacement
- Origine
- Statut

### Actions

- Ajouter pesee du lot
- Enregistrer aliment distribue
- Declarer traitement du lot
- Declarer pertes
- Vendre tout ou partie du lot

## 6. Module Reproduction

## 6.1 Vue reproduction

### Objectif

Suivre les truies et les evenements reproductifs.

### Onglets

- Truies a surveiller
- Saillies recentes
- Gestations
- Mises bas prevues
- Sevrages prevus
- Historique

### Informations affichees

- Truie
- Date de saillie
- Verrat utilise
- Date probable de mise bas
- Statut
- Alerte associee

## 6.2 Ajouter une saillie

### Champs

- Truie
- Verrat
- Date
- Type : naturelle ou insemination
- Observations

### Resultat attendu

- Creation d'un evenement de reproduction
- Calcul automatique de la date probable de mise bas
- Creation d'alertes de suivi

## 6.3 Enregistrer une mise bas

### Champs

- Truie
- Date de mise bas
- Nes vivants
- Mort-nes
- Morts apres naissance si applicable
- Observations

### Resultat attendu

- Mise a jour de l'historique de la truie
- Creation ou mise a jour des porcelets ou du lot
- Programmation d'une alerte de sevrage

## 6.4 Enregistrer un sevrage

### Champs

- Truie ou lot
- Date de sevrage
- Nombre sevre
- Poids moyen si disponible
- Destination : nouveau lot, vente, autre

## 7. Module Sante

## 7.1 Tableau sanitaire

### Objectif

Voir rapidement les problemes sanitaires et les actions a faire.

### Sections

- Animaux malades
- Traitements en cours
- Vaccins a venir
- Vermifuges a venir
- Mortalites recentes
- Medicaments en retrait avant vente

## 7.2 Ajouter un probleme sanitaire

### Champs

- Animal ou lot
- Date
- Symptomes
- Gravite
- Responsable du signalement
- Observation

### Actions suivantes

- Ajouter traitement
- Marquer sous observation
- Appeler veterinaire

## 7.3 Ajouter un traitement

### Champs

- Animal ou lot
- Probleme associe si existant
- Medicament
- Dose
- Date de debut
- Date de fin si connue
- Responsable
- Periode de retrait avant vente
- Observation

### Resultat attendu

- Historique sanitaire mis a jour
- Stock medicament diminue si suivi en stock
- Alerte creee si traitement a renouveler

## 7.4 Declarer une mortalite

### Champs

- Animal ou lot
- Date
- Nombre concerne si lot
- Cause probable
- Observation
- Photo optionnelle dans une version future

### Resultat attendu

- Statut animal modifie ou nombre du lot reduit
- Tableau de bord mis a jour
- Rapport mortalite alimente

## 8. Module Alimentation

## 8.1 Plan alimentaire

### Objectif

Definir les rations selon les categories d'animaux.

### Informations

- Categorie animale
- Aliment principal
- Quantite par jour
- Unite
- Frequence
- Cout estime

## 8.2 Distribution alimentaire

### Champs

- Date
- Animal ou lot
- Aliment
- Quantite distribuee
- Responsable
- Observation

### Resultat attendu

- Stock aliment diminue
- Cout alimentaire calcule
- Historique de consommation mis a jour

## 9. Module Stocks

## 9.1 Liste des stocks

### Categories

- Aliments
- Medicaments
- Vaccins
- Nettoyage
- Materiel

### Informations affichees

- Nom article
- Quantite disponible
- Unite
- Seuil d'alerte
- Date d'expiration si applicable
- Statut : normal, faible, expire bientot, expire

## 9.2 Ajouter une entree de stock

### Champs

- Article
- Categorie
- Quantite
- Unite
- Prix total
- Fournisseur
- Date d'achat
- Date d'expiration si applicable

## 9.3 Sortie de stock

### Champs

- Article
- Quantite sortie
- Motif : alimentation, traitement, perte, nettoyage, autre
- Date
- Responsable

## 10. Module Ventes

## 10.1 Liste des ventes

### Informations affichees

- Date
- Client
- Type : animal, lot, viande, autre
- Quantite
- Montant total
- Montant paye
- Reste a payer
- Statut paiement

## 10.2 Enregistrer une vente

### Champs

- Date
- Client
- Animal ou lot vendu
- Type de vente : par animal, par kg, par lot
- Poids si applicable
- Prix unitaire
- Montant total
- Montant paye
- Mode de paiement
- Date prevue du reste a payer si credit

### Resultat attendu

- Animal marque vendu ou lot reduit
- Chiffre d'affaires mis a jour
- Creance client creee si paiement incomplet

## 11. Module Depenses

## 11.1 Liste des depenses

### Categories

- Aliment
- Medicament
- Vaccin
- Main-d'oeuvre
- Transport
- Entretien
- Energie ou eau
- Achat animal
- Autre

## 11.2 Ajouter une depense

### Champs

- Date
- Categorie
- Montant
- Fournisseur ou beneficiaire
- Mode de paiement
- Description
- Piece jointe dans une version future

## 12. Module Taches

## 12.1 Liste des taches

### Vues

- Aujourd'hui
- En retard
- A venir
- Termine

### Informations affichees

- Titre
- Responsable
- Heure ou date
- Priorite
- Statut

## 12.2 Ajouter une tache

### Champs

- Titre
- Description courte
- Date
- Heure optionnelle
- Responsable
- Priorite
- Repetition : aucune, quotidienne, hebdomadaire, mensuelle
- Lien avec animal ou lot si necessaire

## 13. Module Rapports

### Rapports disponibles en V1

- Etat du cheptel
- Reproduction
- Sante
- Stocks
- Ventes
- Depenses
- Synthese mensuelle

### Filtres

- Periode
- Categorie animale
- Lot
- Responsable

### Formats

- Consultation a l'ecran en V1
- Export PDF et Excel en version suivante

## 14. Parametres

### Sections

- Profil de la ferme
- Utilisateurs et roles
- Devise
- Categories d'animaux
- Types d'aliments
- Medicaments courants
- Fournisseurs
- Clients
- Sauvegarde et synchronisation

## 15. Parcours utilisateur prioritaires

## 15.1 Demarrer avec une nouvelle ferme

1. L'utilisateur cree son compte
2. Il renseigne les informations de la ferme
3. Il choisit la devise et le mode de gestion
4. Il ajoute les premiers animaux ou lots
5. Le tableau de bord devient disponible

## 15.2 Ajouter un lot de porcs en engraissement

1. Ouvrir Cheptel
2. Choisir Ajouter lot
3. Renseigner nom, categorie, nombre, date d'entree, poids moyen et emplacement
4. Enregistrer
5. Le lot apparait dans le cheptel et le total animaux est mis a jour

## 15.3 Suivre une truie jusqu'au sevrage

1. Ouvrir la fiche truie
2. Enregistrer la saillie
3. Consulter l'alerte de mise bas prevue
4. Enregistrer la mise bas
5. Creer le lot de porcelets
6. Recevoir l'alerte de sevrage
7. Enregistrer le sevrage et le nombre de porcelets sevres

## 15.4 Traiter un animal malade

1. Ouvrir Sante
2. Ajouter un probleme sanitaire
3. Choisir l'animal ou le lot concerne
4. Saisir les symptomes
5. Ajouter le traitement
6. Le stock medicament est ajuste
7. Une alerte de suivi est creee

## 15.5 Vendre des porcs

1. Ouvrir Ventes
2. Choisir Nouvelle vente
3. Selectionner animal ou lot
4. Saisir client, quantite, prix et paiement
5. Enregistrer
6. Le cheptel et les finances sont mis a jour

## 16. Priorite des ecrans pour le prototype

Pour construire rapidement une application utilisable, les ecrans a developper en premier sont :

1. Connexion et creation ferme
2. Tableau de bord
3. Cheptel : liste, fiche animal, fiche lot
4. Ajout animal et ajout lot
5. Reproduction : saillie, mise bas, sevrage
6. Sante : probleme, traitement, mortalite
7. Stocks : liste et entree simple
8. Alimentation : distribution
9. Ventes et depenses
10. Rapports simples

## 17. Regles d'ergonomie

- Les formulaires doivent etre courts
- Les champs obligatoires doivent etre limites
- Les boutons principaux doivent etre visibles
- Les listes doivent avoir recherche et filtres
- Les alertes importantes doivent apparaitre sur l'accueil
- Les termes doivent etre compréhensibles par les fermiers
- Les montants doivent afficher la devise locale
- L'application doit rester utilisable avec une connexion instable

## 18. Prochaine etape

La prochaine etape consiste a definir le modele de donnees : tables, champs, relations et logique de base. Ce modele servira a construire la base de donnees puis le prototype fonctionnel.
