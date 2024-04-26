# Etude numérique sur le rapport entre *Zeit* et *Raum* dans la <ins>Critique de la Raison Pure</ins> de Kant

Projet réalisé dans le cadre d'une semaine intensive sur l'Analyse des Réseaux au sein du Master Humanités Numériques de l'Ecole Nationale des Chartes - PSL.

## Conceptualisation

### Questionnement

La question du rapport entre les deux souches de la sensibilité que sont l'espace et le temps dans la <ins>Critique de la Raison Pure</ins> et l'éventuelle priorité de l'un sur l'autre : il s'agit d'une question majeure de l'exégèse kantienne.

L'espace et le temps sont traités en parallèle, pourtant la symétrie se rompt à certains endroits dans le texte.

**En faveur d'une priorité du temps sur l'espace :**
1) Primauté du temps du point de vue de son extension. Tout se donne dans le temps, l'intériorité comme l'extériorité, mais seule l'extériorité se donne dans l'espace.
2) Dans l'<ins>Analytique des Principes</ins> : Le temps permettrait l'usage des catégories dans un jugement synthétique

**En faveur d'une priorité de l'espace sur le temps :**

3. Du point de vue de la compréhension, je ne peux comprendre le temps que par l'espace. Je me rends compte du passage du temps par le mouvement, donc par des déterminations spaciales. L'espace est donc nécessaire pour se représenter le temps.

[Source : Notes du cours  suivi à l'Ecole Normale Supérieure lors du premier semestre de l'année scolaire 2023-2024, donné par Mme Elena Partene, sur la <ins>Critique de la Raison Pure</ins>.]

### Plan de la <ins>Critique de la Raison Pure</ins>

```
Vorrede
Einleitung
I. Transzendentale Elementarlehre
    Erster Teil. Die transzendentale Ästhetik
            § 1
        1. Abschnitt. Von dem Raume
            § 2. Metaphysische Erörterung dieses Begriffs
            § 3. Transzendentale Erörterung des Begriffs vom Raume
        2. Abschnitt. Von der Zeit
            § 4. Metaphysische Erörterung des Begriffs der Zeit
            § 5. Transzendentale Erörterung des Begriffs der Zeit
            § 6. Schlüsse aus diesen Begriffen
            § 7. Erläuterung
            § 8. Allgemeine Anmerkungen zur transzendentalen Ästhetik
    Zweiter Teil. Die transzendentale Logik
        Einleitung. Idee einer transzendentalen Logik
        Erste Abteilung. Die transzendentale Analytik
            Erstes Buch. Die Analytik der Begriffe
            Zweites Buch. Die Analytik der Grundsätze
        Zweite Abteilung. Die transzendentale Dialektik
II. Transzendentale Methodenlehre
```
### Choix pour la modélisation en graphes
* noeuds : noms
* contexte : phrases (sentences) ou paragraphes. Comparaison des résultats selon le contexte choisi.

## Démarche
1. Collecte des données : Téléchargement du format PLAIN TEXT UTF-8 de la Seconde Edition de la <ins>Critique de la Raison Pure</ins> sur le site du Projet Gutenberg (https://gutenberg.org/ebooks/6343). Disponible dans `./data/Corpus_txt/KrV2Aufl.txt`
2. Sélection des sous-documents (un graphe sera produit par document). Disponibles également dans `./data/Corpus_txt`
3. Prétraitement : Transformation des textes en csv où chaque ligne correspond à une phrase ou bien à un paragraphe lié.e à un identifiant (Selon le type d'analyse mené).
4. Génération des graphes : Utilisation de Cortext manager (https://www.cortext.net/projects/cortext-manager/).

## Résultats

### Première Comparaison : <ins>Esthétique Transcendantale</ins>

Les §2-3 portant sur l'espace :
![KrV2Aufl-TrAesthetik-Raum§2-3_paragraph](https://github.com/ASchopenhauer/KrV_ZeitRaum_NetSci/assets/153139719/3f8b16f3-5f50-4878-9c71-b79de03e2952)

Les §4-7 portant sur le temps :
![KrV2Aufl-TrAesthetik-Zeit§4-7_paragraph](https://github.com/ASchopenhauer/KrV_ZeitRaum_NetSci/assets/153139719/62ff0b25-4511-4620-b4ee-8b1013587ff0)

### Deuxième Comparaison : Croisement des structures

![RECONST-MetEroerterung-RaumZeit_2-4_sentence](https://github.com/ASchopenhauer/KrV_ZeitRaum_NetSci/assets/153139719/2467f39f-c5ce-49c5-8b02-19201533e6d1)

### Troisième Comparaison : Rôle de *Zeit* et *Raum* dans l'<ins>Analytique des Principes</ins>

Vue d'ensemble :
![KrV2Aufl-TrLogik-TrAnalytik-AnalGrundsaetze_nett_sentence](https://github.com/ASchopenhauer/KrV_ZeitRaum_NetSci/assets/153139719/9a49dd5d-58a9-47cc-b34a-a4b7efb55bdc)


Le temps :
![KrV2Aufl-TrLogik-TrAnalytik-AnalGrundsaetze_nett_focusZeit_sentences](https://github.com/ASchopenhauer/KrV_ZeitRaum_NetSci/assets/153139719/269ece07-c375-4245-9bc2-76f32ec5b543)

L'espace :
![KrV2Aufl-TrLogik-TrAnalytik-AnalGrundsaetze_nett_focusRaum_sentence](https://github.com/ASchopenhauer/KrV_ZeitRaum_NetSci/assets/153139719/c70b19fe-1eb0-4f08-8b6a-3db0e413f28d)


<ins>**Observations**</ins>: Le temps semble avoir plus d'importance dans cette partie du texte.


