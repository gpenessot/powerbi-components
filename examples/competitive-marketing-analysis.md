---
layout: project
title: "Competitive Marketing Analysis"
date: 2026-05-22
tags: [Power BI, Data Visualisation, Marketing]
---

Dashboard interactif d'analyse marketing concurrentielle, basé sur le rapport exemple
officiel de Microsoft Power BI.

## Objectif

Comparer les performances commerciales par canal de distribution (Online, Social Media,
Stores, Outlet) et par produit, afin d'identifier les leviers de croissance et d'optimiser
l'allocation des investissements marketing.

{% include powerbi-dashboard.html
  title="Competitive Marketing Analysis"
  description="Ventes totales $32K — répartition par canal, ROI et tendances mensuelles."
  embed_url="https://app.powerbi.com/view?r=eyJrIjoiYmY0YzI5MTItODQ2Yy00YmY3LTk3NTMtYmQ4MDE5MDMyYThjIiwidCI6IjAxZDJkNTg3LTM1YTctNGFkYy1iNGM3LTFmZTgxYjYzZDY1ZSJ9"
  data_source="Microsoft Power BI Desktop Samples"
  source_url="https://github.com/microsoft/powerbi-desktop-samples"
  height="540px"
%}

## Insights Clés

- Le canal **Online** représente 45,84 % des ventes ($15K) avec un ROI de 12 %.
- **Social Media** génère $9 262 (28,92 %) mais affiche un ROI de 0 % — canal à optimiser.
- **Outlet** ne pèse que 4,18 % des ventes mais dégage le meilleur ROI : 18 %.
- Le produit **Maximus UM-70** est le best-seller Online avec $2 359 de ventes.
- Les ventes Online atteignent leur pic en **octobre–novembre**, suggérant un effet saisonnier.

## Source

Rapport exemple fourni par Microsoft :
[Competitive Marketing Analysis.pbix](https://github.com/microsoft/powerbi-desktop-samples/blob/main/new-power-bi-service-samples/Competitive%20Marketing%20Analysis.pbix)
