# SAP_macro_and_script
Macro was designed to help find and calculate value of special stock - manufactured products which are used as maintenance stock
For such supplies, mentioned macro will gather data such as material ID, plant number, Profit Center etc. to help prepare journal correction to write them off.

Despite macro's aim to improve ERSA process, it has some limitation. For now maximum number of plants available to process in one run is 8, and maximum number of materials from storage locations 8000-8999 is 3999. It also use all of excel file sheets, so user is requested to do not make any changes in macro's layout.

If you use macro before, please check if your "TEMP" folder do not contain any temporary data from previous runs.
If yes, please delete that (for more details, please take a look at the end of this instruction).

The first step to configure macro is to update information: company code, current year & month and specify all Mfg plants for particular company code - please insert data into dark grey cells. Other data like t-code, table name, storage locations range, temporary data (from SE16 tables) files name and technical field names are also set as variables however it is not recommended to make any changes, because it could interrupt macro's activity.

After initial update of data, please open SAP on default panel go through listed below buttons in order. For steps 2-5, after clicking "ok" on message checkbox, please wait until table data file generate and minimalize it Please put attenton on steps 3-4 - after each of them you will get info if there is reason of processing further steps. For step 6, please click "no" on incoming message checkbox.

After completing running macro, please delete temporary data files from listed below location. Please also save created ERSA file into desired location and then delete it from folder "TEMP".
