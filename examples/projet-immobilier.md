---
layout: project
title: "Analyse du Marché Immobilier Parisien"
date: 2026-01-15
tags: [Power BI, Data Visualisation, Open Data]
---

# Analyse du Marché Immobilier Parisien

Exploration interactive des transactions immobilières à Paris entre 2020 et 2024,
à partir des Demandes de Valeurs Foncières (DVF) publiées sur data.gouv.fr.

## Objectif

Identifier les arrondissements avec le meilleur rapport qualité/prix et les
tendances de marché pour les primo-accédants.

{% include powerbi-dashboard.html
  title="Marché Immobilier Paris — DVF 2020–2024"
  description="Prix au m² par arrondissement, volume de transactions, évolution annuelle."
  embed_url="https://app.powerbi.com/view?r=REMPLACEZ_PAR_VOTRE_CODE"
  data_source="DVF — data.gouv.fr"
  source_url="https://www.data.gouv.fr/fr/datasets/demandes-de-valeurs-foncieres/"
  height="650px"
%}

## Insights Clés

- Le prix médian au m² a progressé de X% entre 2020 et 2024 dans le 11e.
- Les studios offrent un rendement locatif supérieur aux grands appartements.
- Le marché s'est nettement ralenti depuis le T3 2023.
