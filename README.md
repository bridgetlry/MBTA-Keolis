# MBTA-Keolis

Created during my time as a Data Analytics Co-op in the Procurement and Logistics Department at the MBTA.


This script transforms the raw inventory monthly data received from Keolis Commuter Services into comprehensive files with information on transaction history and overall inventory on hand. This configuration was previously done manually using Microsoft Excel and Microsoft Access but now uses a more succinct Python notebook.

The `pandas`, `numpy`, and `shutil` libraries may need to be installed on whichever software you use prior to running the script. The data is first reshaped to match a preexisting template that keeps the columns organized in the event of the raw data being formatted differently. It is then evaluated by a series of queries that filter out and modify specific fields all while creating three data frames (`All_Txns`, `Initial_Inv`, `Initial_Final`) that serve as outputs to be used in Tableau Prep Builder, the final step of creating the Keolis Monthly Inventory Report.

The Data Analytics Team in the Procurement and Logistics Department at the MBTA can run this code each month to conveniently prepare and clean data to eventually use in the Tableau report. 

This code is updated as of August 2nd, 2023 but is subject to becoming outdated if any future co-ops make modifications or develop additional features.

*NOTE*: this can only be run on the MBTA server, as it references files on a Common Drive, hence the format of a Python notebook so the data frame outputs can be seen after cells.
