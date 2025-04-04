# DP-203_Lab2
# Bestanden opvragen met Serverless SQL Pools in Azure Synapse Analytics

Dit project laat zien hoe je **Azure Synapse Analytics Serverless SQL Pools** kunt gebruiken om gestructureerde en semi-gestructureerde data in een **Data Lake** op te vragen, zonder dat je een traditionele database nodig hebt.

## 🧠 Doelstelling

Leer hoe je bestanden in CSV-, Parquet- en JSON-indeling kunt opvragen met SQL via de serverless SQL pool in Synapse Studio. Je leert:
- Een Synapse-werkruimte inrichten
- Data in verschillende bestandsindelingen verkennen
- Bestanden opvragen met `OPENROWSET`
- Externe gegevensbronnen en tabellen maken
- Resultaten visualiseren in Synapse Studio

---

## 🛠️ Vereisten

- Een actieve **Azure-abonnement** met beheerdersrechten
- Basiskennis van SQL
- Bekendheid met Azure Portal en Synapse Studio

---

## ⚙️ Installatieproces

1. **Inrichten van Synapse Analytics Workspace**  
   - Gebruik Azure Cloud Shell (PowerShell) om een lab-repository van GitHub te klonen
   - Voer een installatiescript uit om een Synapse-werkruimte te maken en voorbeeldgegevens naar Azure Data Lake te uploaden

2. **Controleer Data Lake-structuur in Synapse Studio**  
   - Ga naar Synapse Studio en controleer of de data lake de volgende mappen bevat:
     - CSV-bestanden
     - JSON-bestanden
     - Parquet-bestanden

---

## 🔍 Bestanden opvragen met Serverless SQL

### 1. CSV-bestanden opvragen
- Gebruik `OPENROWSET` om data uit `.csv`-bestanden te lezen
- Bekijk eerst de ruwe resultaten zonder kolomnamen
- Maak het leesbaarder door een schema toe te passen met een `WITH`-clausule

### 2. Parquet-bestanden opvragen
- Gebruik wildcard-paden om gesplitste `.parquet`-bestanden op te vragen
- Voer aggregaties uit, zoals het tellen van bestellingen per jaar
- Filter op partities direct via het bestandspad

### 3. JSON-bestanden opvragen
- Lees JSON als tekst en gebruik `JSON_VALUE` om velden uit te pakken
- Gebruik aangepaste delimiters om regel-voor-regel te lezen
- Projecteer velden zoals SalesOrderNumber en CustomerName

---

## 🧱 Externe gegevensobjecten maken

### 1. Externe gegevensbron
- Maak een database in de serverless SQL pool
- Definieer een `EXTERNAL DATA SOURCE` die verwijst naar de data lake

### 2. Externe tabellen
- Definieer bestandsindelingen (`EXTERNAL FILE FORMAT`)
- Maak `EXTERNAL TABLES` die data uit CSV-bestanden weergeven
- Voer queries uit op externe tabellen alsof het gewone SQL-tabellen zijn

---

## 📊 Data visualiseren

- Gebruik de **Chart**-functie van Synapse Studio om resultaten te visualiseren
- Voorbeeld: Visualiseer `GrossRevenue` per jaar met een lijn- of kolomdiagram

---

## 🧹 Opruimen

- Verwijder de resource group die tijdens het lab is aangemaakt om kosten te vermijden
- Dit verwijdert de Synapse-werkruimte, de data lake en alle gekoppelde resources

---

## 📎 Referenties

- [Serverless SQL pool in Azure Synapse Analytics](https://learn.microsoft.com/nl-nl/azure/synapse-analytics/sql/on-demand-overview)
- [OPENROWSET in Synapse SQL](https://learn.microsoft.com/nl-nl/azure/synapse-analytics/sql/query-data-storage-files)

---

## 📁 Projectbron

Dit project is gebaseerd op het Microsoft Learning-pad voor de **DP-203 Azure Data Engineer** certificering.
![Schermafbeelding 2025-04-04 215620](https://github.com/user-attachments/assets/208b48bd-263d-46d0-9820-09607cf22327)
![Schermafbeelding 2025-04-04 215709](https://github.com/user-attachments/assets/2dedde13-2516-4462-82f6-1bb2483f44f8)
![Schermafbeelding 2025-04-04 215835](https://github.com/user-attachments/assets/6635aaf1-de2f-4b31-8877-fa3fca9026f1)
![Schermafbeelding 2025-04-04 220843](https://github.com/user-attachments/assets/d325aec5-11f8-4798-808a-a8c72bce0952)
![Schermafbeelding 2025-04-04 222455](https://github.com/user-attachments/assets/ac3d53f9-35d8-406b-b6aa-f69429345b9d)
![Schermafbeelding 2025-04-04 223338](https://github.com/user-attachments/assets/c9297e1f-0a02-49d8-a6b7-cdff5e6affcb)
![Schermafbeelding 2025-04-04 223551](https://github.com/user-attachments/assets/f7f0f098-2a2b-4949-96ff-43f840cad5f0)
![Schermafbeelding 2025-04-04 223755](https://github.com/user-attachments/assets/34269c59-4de3-4fc1-8e9e-08bf178390cc)
![Schermafbeelding 2025-04-04 223828](https://github.com/user-attachments/assets/8bd8e9ef-d511-48b8-9f1c-1a7bb0660542)









