---
description: Betreft invulvelden Adlib/Axiell Collections die geïmporteerd worden in DAMS
---

# Mapping Personen en Instellingen

| VELD | OSLO | HVA | IM | DMG | STAM | AG |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| naam | volledigeNaam | HVA | IM | DMG | STAM | AG |
| naam.soort |  | HVA | IM | DMG | STAM | AG |
| referentienummer | Object.identificator | HVA | IM | DMG | STAM | AG |
| use | skos:related | HVA | IM | DMG |  |  |
| used\_for | skos:related | HVA | IM | DMG |  |  |
| titel | alternatieveNaam |  |  |  |  | AG |
| geslacht | geslacht | HVA |  | DMG | STAM | AG |
| achternaam | achternaam | HVA |  | DMG | STAM | AG |
| voornaam | voornaam | HVA |  | DMG | STAM | AG |
| aanhef | alternatieveNaam |  |  |  |  | AG |
| bron |  | HVA | IM | DMG | STAM | AG |
| bron.nummer |  | HVA | IM | DMG | STAM | AG |
| naam.status |  | HVA | IM | DMG | STAM | AG |
| geboorte.datum.begin | heeftGeboorte | HVA | IM | DMG | STAM | AG |
| geboorte.datum.eind |  |  |  | DMG | STAM | AG |
| geboorte.plaats | heeftGeboorte --&gt; plaats | HVA | IM | DMG | STAM | AG |
| overlijden.datum.begin | heeftOverlijden | HVA | IM | DMG | STAM | AG |
| overlijden.datum.eind |  |  |  | DMG | STAM | AG |
| overlijden.plaats | heeftOverlijden --&gt; plaats | HVA | IM | DMG | STAM | AG |
| nationaliteit | heeftNationaliteit | HVA |  | DMG | STAM | AG |
| beroep | Agent.voerdeUit | HVA |  |  |  | AG |
| plaats\_werkzaamh |  |  |  |  |  | AG |
| plaats\_activiteit.instituut |  |  |  |  |  | AG |
| biografie |  | HVA |  |  |  | AG |
| structuur/genealogie | alternatieveNaam |  |  |  |  | AG |
| relatie.bijzonderheden |  |  |  |  |  | AG |
| related\_term |  |  |  |  |  | AG |
| relatie.categorie |  |  |  |  |  | AG |

