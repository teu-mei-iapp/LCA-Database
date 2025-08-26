<div style="display: flex; align-items: center; justify-content: space-between; width: 100%;">
  <h1>LCA-Database</h1>
  <img src="https://github.com/user-attachments/assets/35cc3edb-4195-45e8-9562-680798594199" alt="BayflexLogo" width="100"/>


</div>





<div style="display: flex">
  <div class="blurb">
    <h1>LCA-Database</h1
  </div>
  <div id="PhotoOfMe" style="margin-left:10px">
    <img src="https://github.com/user-attachments/assets/35cc3edb-4195-45e8-9562-680798594199" alt="BayflexLogo" width="100"/>
  </div>
</div>
An open-source database for Life-Cycle Assessment (LCA) and Process of Record (PoR) of fabrication systems in flexible and printed electronics.
This database is designed to evolve continuously through contributions from the research community.

**Notice:** All scientific publications making use of this repository should cite the associated paper.
Further information on the PoR and the LCA - including definitions, general structure, and objectives - can be found therein.
> L. Teuere, T. Meier, H. Kleemann, et al. <br>
> *Life-Cycle Assessment of Printed Electronic Components – Case Study for Organic Electrochemical Transistors*.  
> _Advanced Electronic Materials_, accepted (2025).
> 

**Contact:** lca.repository.iapp@outlook.com

<br>
<br>

**General Disclaimer**<br>
The aim of this database is to gather and document LCA Data for common fabrication processes and chemicals in the field of microelectronics, with a focus on organic and printed electronics. While we aim to bridge a gap of missing Flows in common databases, a license for one of them (e.g. ecoinvent https://ecoinvent.org/) as well as any LCA software (e.g. openLCA https://www.openlca.org/) is still required to properly conduct a Life-Cycle Analysis to gain access to data for common chemicals and background processes, as well as impact assessment methods, required for calculations. The data for the Processes, Machines, and Materials in this database can give you a point to start your own LCA, but we advise you to modify existing Processes to your actual fabrication schemes. These include, but are not limited to, actual machine power and run times, as well as ink consumption.

**Community Contributions**<br>
We invite you to contribute to the databse yourself


**Structure of the LCA Database**<br>
The LCA Database contains a structure of grouped LCA tables containing Fabrication and System Processes and Flows connected to the Process of Record.
You can find:<br>
 → Full Processes for listed Product and Fabrication System Processes<br>
 → Specialized Fabrication Processes (e.g. plasma or parylene processes)<br>
 → Specialized Chemicals used in Fabrication<br>
 → Machines and corresponding use times<br>
*A full overview over the contents of the tables is found in the overview_tables.txt*<br>

For any Processes you want to contribute to this Database, we will assign a new label and name corresponding to the existing scheme of the Process of Record.


**Add tables to your own LCA tool**<br>
The input and output Flow data from this LCA database has to be manually copied into preferred LCA tool (e.g. openLCA)<br>
-	Create a new Process and a quantitative Reference Flow. Make sure to select the correct reference Flow Property as given in the Github-table (e.g. Mass, Duration, Number of items).<br>
-	Copy the input and output Flows from the Github-tables with the correct amount and unit each.<br>
<img width="577" height="349" alt="grafik" src="https://github.com/user-attachments/assets/0b466db9-5cf7-44b2-aa01-1dedc3613fd3" />


-	Make sure to correctly define the Reference Flow (e.g. Process for 1h of machine time or 1 item).<br>
 → Some Processes require input Flows, that are also defined in the Github-tables and are not found in usual databases. These are marked with an asterisk * in the tables.<br>
*Optional*: add Process and Flow descriptions to complete your database entry. The Processes are fully workable with Input and Output Flows set correctly.<br>

*If you can prove ownership of a valid ecoinvent license, you can request the directly exported JSON files for the database or specific processes.*<br>

**Add a blank GWP value for a new material**<br>
-	Create a new Process and a quantitative reference Flow, which should be 'Mass'.<br>
-	Add carbon dioxide emission, fossil as an additional output Flow with the representative GWP value ('number [kg CO2-Eq.]') for 1kg of the new material.<br>
<img width="574" height="271" alt="grafik" src="https://github.com/user-attachments/assets/8e6639fb-b9b0-4a47-bd78-302dc7dd2f35" />

**Add a specific electricity value for your country**<br>
-	Create a new Process and a quantitative reference Flow, which should be 'Energy'.<br>
-	Add carbon dioxide emission, fossil as an additional output Flow with the representative GWP value ('number [g CO2-Eq.]') for 1 kWh in your country.<br>
<img width="436" height="270" alt="grafik" src="https://github.com/user-attachments/assets/3bcc888c-dab0-4c75-8451-d5f16caf3a8b" />



# vorgefertigte Prozesse von hier gerne anpassen an eigene 'richtige' Verbrauchswerte

