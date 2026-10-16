# National Bank of Canada Stock Analysis (Power BI)

![Dashboard](dashboard.png)

## Overview

Power BI dashboard analyzing the stock price of National Bank of Canada (NA.TO, Toronto Stock Exchange) over one year, from October 2025 to October 2026.

## Data

- Source: Yahoo Finance, NA.TO historical data (daily prices, 1 year)
- The raw data is not included in this repository due to Yahoo Finance terms of use.

## Data cleaning (Power Query)

- Checked and set column headers.
- Removed dividend rows mixed with price data.
- Converted price columns from text to decimal numbers using English (United States) regional settings, since the source uses a period as the decimal separator.
- Detected abnormal values in the Volume column (for example, 995 instead of 995,200). The cause was a format conflict: a French-language Excel read the thousands separator as a decimal comma. After confirming with the source, I removed the column rather than use incorrect data.

## Dashboard

- Line chart showing the daily closing price over one year
- Key indicators: highest price, lowest price and average price
- Short written summary of the trend

## Key findings

- The stock rose from $151.72 to $204.20 over the year, an increase of about 35%.
- It reached a high of $235.32 in July 2026, then declined gradually until October.
- The average closing price over the period was $193.32.

## Tools

Power BI Desktop, Power Query, Excel

---

# Analyse de l'action Banque Nationale (Power BI)

## Aperçu

Tableau de bord Power BI analysant l'évolution du cours de l'action Banque Nationale (NA.TO, Bourse de Toronto) sur un an, d'octobre 2025 à octobre 2026.

## Données

- Source : Yahoo Finance, données historiques de NA.TO (prix quotidiens, 1 an)
- Les données brutes ne sont pas incluses dans ce dépôt, en raison des conditions d'utilisation de Yahoo Finance.

## Nettoyage des données (Power Query)

- Vérification et définition des en-têtes de colonnes.
- Suppression des lignes de dividendes mêlées aux prix.
- Conversion des colonnes de prix du texte en nombres décimaux avec les paramètres régionaux Anglais (États-Unis), puisque la source utilise le point comme séparateur décimal.
- Détection de valeurs anormales dans la colonne Volume (par exemple, 995 au lieu de 995 200). La cause était un conflit de format : Excel en français avait lu le séparateur de milliers comme une virgule décimale. Après vérification auprès de la source, j'ai retiré la colonne plutôt que d'utiliser des données incorrectes.

## Tableau de bord

- Graphique en courbes du prix de clôture quotidien sur un an
- Indicateurs clés : prix le plus haut, prix le plus bas et prix moyen
- Courte conclusion écrite sur la tendance

## Principaux constats

- L'action est passée de 151,72 $ à 204,20 $ sur l'année, soit une hausse d'environ 35 %.
- Elle a atteint un sommet de 235,32 $ en juillet 2026, puis a reculé progressivement jusqu'en octobre.
- Le prix de clôture moyen sur la période est de 193,32 $.

## Outils

Power BI Desktop, Power Query, Excel
