# MBTA-Keolis

This script transforms the raw inventory monthly data received from Keolis Commuter Services into comprehensive files with information on transaction history and overall inventory on hand. This configuration was previously done manually using Microsoft Excel and Microsoft Access but now uses a more succinct Python notebook.

The data is first reshaped to match a preexisting template that keeps the columns organized in the event of the raw data being formatted differently. It is then evaluated by a series of queries that filter out and modify specific fields all while creating three data frames (All_Txns, Initial_Inv, Initial_Final) that serve as outputs to be used in Tableau Prep Builder, the final step of creating the Keolis Monthly Inventory Report.
