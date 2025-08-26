# LCA-Database

An open-source database for an Life-Cycle Assesement (LCA) for flexible and printed electronics.

**Notice:** All scientific publications making use of this repository should cite the associated paper.
> L. Teuere, T. Meier, H. Kleemann, et al. <br>
> *Life-Cycle Assessment of Printed Electronic Components – Case Study for Organic Electrochemical Transistors*.  
> _Advanced Electronic Materials_, accepted (2025).
> 

**Contact:** lca.repository.iapp@outlook.com

**General Disclaimer**<br>
The aim of this database is to gather and document LCA Data for common fabrication processes and chemicals in the field of microelectronics, with a focus on organic and printed electronics.<br>
While we aim to bridge a gap of missing Flows in common databases, a license for one of them (e.g. ecoinvent https://ecoinvent.org/) is still required to properly conduct a Life-Cycle Analysis to gain access to data for common chemicals and background processes, as well as impact assessment methods, required for calculations.
#kurzes Statement über Datenbanken vs software (was wird required)
#Vermerk auf Paper, aber kein generelles Tutorial über Softwarenutzung -> link zu openLCA Doc

**Structure of the LCA Database**<br>
The LCA Database contains a structure of grouped LCA tables containing Fabrication and System Processes and Flows connected to the Process of Record.
You can find:<br>
 → Full Processes for listed Product and Fabrication System Processes<br>
 → Specialized Fabrication Processes (e.g. plasma or parylene processes)<br>
 → Specialized Chemicals used in Fabrication<br>
 → Machines and corresponding use times<br>
*A full overview over the contents of the tables is found in the overview_tables.txt*<br>

**Add tables to your own LCA tool**<br>
The input and output Flow data from this LCA database has to be manually copied into preferred LCA tool (e.g. openLCA)<br>
-	Create a new Process and a quantitative Reference Flow. Make sure to select the correct reference Flow Property as given in the Github-table (e.g. Mass, Duration, Number of items).<br>
-	Copy the input and output Flows from the Github-tables with the correct amount and unit each.<br>
 <img width="850" height="366" alt="grafik" src="https://github.com/user-attachments/assets/891c3fee-70e6-4712-9e30-4cfa162a5aa9" />

-	Make sure to correctly define the Reference Flow (e.g. Process for 1h of machine time or 1 item).<br>
 → Some Processes require input Flows, that are also defined in the Github-tables and are not found in usual databases. These are marked with an asterisk * in the tables.<br>
*Optional*: add Process and Flow descriptions to complete your database entry. The Processes are fully workable with Input and Output Flows set correctly.<br>

*If you can prove ownership of a valid ecoinvent license, you can request the directly exported JSON files for the database or specific processes.*<br>

**Add a blank GWP value for a new material**<br>
-	Create a new Process and a quantitative reference Flow, which should be 'Mass'.<br>
-	Add carbon dioxide emission, fossil as an additional output Flow with the representative GWP value ('number [kg CO2-Eq.]') for 1kg of the new material.<br>
<img width="701" height="309" alt="grafik" src="https://github.com/user-attachments/assets/746211aa-425b-4dff-9f3b-c038f782ef34" />





