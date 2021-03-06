# TableExtension written by gilaga4815 and CreeperAlex309.

Translated by itsdrawn / draaawn.

Module created with the help of many programming articles and devforum documentation with useful methods.

This module serves as an extension for existing table functions to be able to clean up some functions that are reused.

Any function without credits assumes it was written by gilaga4815.

---

## Methods

### tableModule.find
```lua
--- Finds an item in a table
-- @param {table} tab the table
-- @param {any} val the value to index by
-- @return[1] {boolean} if found in table
-- @return[2] {any} the value found in table
tableModule.find = function(tab, val) end
```

---

### tableModule.dictionaryCompare
```lua
--- Runs a shallow comparison on a table (dictionary)
-- @param {table} dict1 the first dictionary
-- @param {table} dict2 the second dictionary
-- @return[1] {boolean} if dictionaries are equal
tableModule.dictionaryCompare = function(dict1, dict2) end
```

---

### checkForNonExistentData
Credits : CreeperAlex309

Parameters of checkForNonExistentData: 

	returnDict - The dictionary you want to return with the added indexes.
	checkDict - The dictionary you want to use as the check for returnDict.
	
This method exists to add or remove indexes of checkDict that is not present in baseDict.

---

### deepCopy
Credits to the original idea: IgnisRBX @ ROBLOX Developer Relations.
Parameters of the deepCopy method:

	Tab - The table you would like to be deepcopied.
	
This method copies the current table passed. But, it also copies every key in the table for embedded tables.

---

### shallowCopy
Credits to the original idea: IgnisRBX @ ROBLOX Developer Relations.
Parameters of the deepCopy method:

	Tab - The table you would like to be shallowcopied.
	
This method copies the table passed. But, it does not copy embedded tables.

---

### clear

Parameters of the clear method:

	Tab - The table you would like to clear.

This method clears every index in its given table.

---

### getPrecedence

Parameters of the getPrecedence method:

	Tab -  The table you would like to request the next index from.
	
This method goes through the table and tells you the next index relative to its current position. If its current index is at the end of the table, it will return the first index in the table.

---

### generateChunks
Credits to the original idea: Ryan Farney @ dev.to

Paremeters of the generateChunks method:

 	Tab -  The table you want to generate chunks from.

This method iterates through all elements inside the table, searching through all of the elements and checking if there is any subtable or if the previous indice is at the users request. If so, a new table is added at the end of the specified table and if it is not the same size as the elements, more are added without adding a new subtable to it. 

---

### stringifyTable

Parameters of the stringifyTable method:

 	Tab - the table of the elements you want to mutate into a string.
	
---

### reverse
Credits to the original idea: sleitneck (crazyman32) @ ROBLOX Devfourm.

Parameters of the reverse method:

	Tab - The table you specify, but in reverse order.

This method reverses the elements in a table, putting the first index at the last & vise versa.

Warning: This returns a shallowcopy and doesn't actually update the table you are inputting.

---
