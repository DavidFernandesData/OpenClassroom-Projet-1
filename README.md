# OpenClassroom-Projet-1
Grand Marché — Rapport marketing mensuel & analyse clients affiliés

Projet pédagogique (OpenClassrooms) — Data Analyst, service Marketing du Grand Marché (grande distribution : alimentaire, biens de consommation)

🧭 Aperçu

Ce dépôt accompagne la mission mensuelle :

préparer une présentation de 5 diapositives basée sur des graphiques mensuels existants, pour expliquer les performances (baisse du CA, perspectives, storytelling clair pour non‑initiés) ;

compléter et mettre à jour un tableau de bord Excel sur les clients affiliés (février), avec 5 visuels dont 1 infographie, en respectant les bonnes pratiques d’accessibilité et en conservant les formules.

🎯 Objectifs pédagogiques

Sélectionner, interpréter et expliquer des KPIs marketing (ventes, CA, panier, visites, conversions, etc.).

Construire un récit court, visuel et actionnable pour la direction.

Mettre à jour un dashboard Excel multi-feuilles (données + synthèse visuelle) et garantir sa maintenabilité.

Proposer un axe stratégique après l’arrêt du segment High Tech (focalisation sur alimentaire & biens de conso).

📦 Livrables attendus

slides/rapport_mensuel_5_slides.pdf (ou .pptx) — 1 graphique / slide, langage simple, recommandations.

excel/dashboard_clients_affilies.xlsx — trame fournie complétée :

MàJ chiffres de février & temps d’achat ;

4 graphiques + 1 infographie (feuille « Tableau de bord ») ;

Feuille 2 : tableau récap par client (nb d’achats, CA, total).

notes/approche_methodo.md — hypothèses, calculs KPI, méthode de prévision, choix de dataviz.

🔢 KPIs & définitions (référentiel)

CA (chiffre d’affaires) : Σ (prix × quantités) sur la période.

Ventes : nb d’unités vendues / nb de commandes (préciser l’unité retenue).

Panier moyen : CA / nb de commandes.

Taux de conversion : nb d’achats / nb de visites.

Visites : sessions web sur la période.

Temps passé (sessions avec achat) : moyenne/variance/déviation standard sur ces sessions uniquement.

Part des ventes par catégorie : CA (ou quantités) par catégorie / total.

Garder ces définitions identiques entre slides & Excel pour éviter les incohérences.

🧩 Étape 1 — Rapport mensuel (5 slides max)

Demande du Directeur Marketing (Frédéric)
Expliquer d’où vient la baisse du CA et comment la situation va évoluer dans les prochains mois.
Utiliser des graphiques mensuels pour couvrir :
Proportion des ventes par catégorie (focus : alimentaire & biens de conso ; High Tech arrêté N‑1).
Montant des achats des clients (panier).
Évolutions dans le temps : CA ; nb d’achats ; ratio achats/visites (≈ conversion) ; nb de visites ; variabilité du temps passé (sessions avec achat).
Temps passé (niveau, distribution) pour les sessions avec achat.
Projection du CA (prochains mois).
Storyline suggérée (exemple)
Où on en est : répartition par catégorie & dynamique globale.
Ce qui bouge : trafic, conversion, panier — qui explique quoi dans la variation du CA.
Comportement d’achat : temps passé, signe d’intention/ friction.

Projection : tendance (saisonnalité possible), scénario prudent/central/optimiste.

Actions : 3 recommandations concrètes (cf. section « Stratégie »).

Idées de dataviz

Part par catégorie : barres empilées ou treemap (1 seule).

Panier : ligne (M‑1 à M) + repères de seuils.

Conversion & visites : deux lignes sur axes distincts ou 2 slides séparées pour rester 1 graphe/slide.

Variabilité du temps : boîte à moustaches (boxplot) ou écart-type par mois.

Projection CA : ligne avec intervalle de confiance (méthode ci‑dessous).

Méthode de projection (simple & transparente)

Point de départ : tendance linéaire ou moyenne mobile (3 à 6 mois) selon stabilité.

Option : décomposition tendance + saisonnalité (si ≥ 12 mois d’historique).

Toujours afficher l’incertitude (IC/borne min‑max) et préciser les hypothèses.

Recommandations de forme

1 slide = 1 message clé ; titre conclusif (ex. « Le CA recule ‑4,2% porté par la chute du trafic »).

Légendes claires, unités visibles, axes annotés ; éviter jargon.

Ajouter notes orateur (résumé de 2‑3 phrases max / slide).

📊 Étape 2 — Clients affiliés (Excel)

Demande de Pauline (Marketing)

Compléter février : chiffres & temps d’achat.

Feuille Tableau de bord : créer 4 graphiques + 1 infographie ; mettre à jour le 1er graphe avec février.

Feuille 2 : tableau récap par client (nb d’achats, CA, total).

Conserver toutes les formules (pour revue & pérennité).

Conseils de mise en œuvre

Garder une feuille Données propre (colonnes datées AAAA‑MM, formats cohérents, pas de cellules fusionnées).

Protéger la feuille « Tableau de bord » (verrouillage léger) tout en laissant les contrôles de filtre.

Visuels possibles :

Top clients (barres triées) ;

Évolution du CA affiliés (ligne) ;

Répartition par segment client (barres empilées / donut avec parcimonie) ;

Fréquence d’achat (histogramme) ;

Infographie : carte KPI (Cartes/Shapes) avec 3 tuiles : CA, Nb achats, Panier moyen.

Accessibilité : tailles ≥ 12pt, contraste suffisant, palettes daltonisme‑friendly, titres explicites.

Feuille 2 — Tableau récap (exemple de colonnes)

client_id | nom_client | nb_achats | CA | panier_moyen | derniere_achat | statut

Ajouter totaux en bas & slicers (mois, segment).

🧪 Checklist qualité

🔐 Conformité & données

Respecter RGPD (fichiers anonymisés / pseudonymisés si exportés).

Versionner les fichiers Excel lourds via LFS (si nécessaire) ou publier uniquement des exports.

🔧 Reproductibilité 

Si vous utilisez des scripts (Python/R) pour préparer des graphes :

Documenter les sources (data/raw/), le nettoyage (data/interim/).

Exporter les images vers slides/ pour insertion dans PowerPoint.

Conserver un notes/approche_methodo.md avec vos formules & choix.

📝 Nommage & versions

rapport_YYYY-MM_v1.pptx ; dashboard_affilies_YYYY-MM.xlsx.

Utiliser un CHANGELOG succinct dans notes/.

📣 Remerciements

Brief & trame fournis par Frédéric (Directeur Marketing) & Pauline (Marketing).

📜 Licence

Ce dépôt est fourni à des fins pédagogiques
