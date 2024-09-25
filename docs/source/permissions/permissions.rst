Permission System
=================

.. warning::

  This page is still under-construction!
  
  Some information could be missing.

The permission system was created to allow the user of custom script to control what a script can do.

When a developer create a custom script / plugin, they need to ask for permissions before using a lot of methods, if the script try to access a method that was not asked before by a permission, the script will not work as the software didn't give the permission to do it.

There is 3 levels of permission:
- Low-level: Those permissions will just show a message box to the user where the user can allow all, some or none.
- Medium-level: Those permissions are more powerfull than low-level, so the user will get a warning message before accepting the permission.
- High-level: Those permissions are **VERY** powerfull, they can remove file, create new file, access internet,... So the user will get a warning message where he need to wait 5 seconds and write a text in a box before having the right to accept.

If a user refuse to give the permission to a script, the script can ask again **one** time only, after that, the script will not be able to ask anymore and the user will need to allow it manually in the software settings.

Low-Level Permissions
---------------------

- UI > Give the ability to the script to create custom UI nodes.

- REGISTERS > Give the ability to the script to access to all register of the software

  - REGISTERS:UI > Give the ability to the script to access to the "UI Register".

  - REGISTERS:CHARACTER > Give the ability to the script to access the "Characters Register".

  - REGISTERS:EFFECT > Give the ability to the script to access the "Effects Register".

  - REGISTERS:ENUM > Give the ability to the script to access the "Enums Register".

  - REGISTERS:HISTORY > Give the ability to the script to access the "History Register".

  - REGISTERS:ITEM_PARAMETERS > Give the ability to the script to access the "Item Parameters Register".

  - REGISTERS:ITEM > Give the ability to the script to access the "Item Register".

  - REGISTERS:SKILL_CONDITION > Give the ability to the script to access the "Skill Condition Register".

  - REGISTERS:SKILL > Give the ability to the script to access the "Skill Register".

- ITEM_EVENTS > Give the ability to the script to link custom function to item event (new_item, delete_item, edit_item, select_item)

  - ITEM_EVENTS:NEW_ITEM > Give the ability to the script to link custom function to the "new_item" event.

  - ITEM_EVENTS:DELETE_ITEM > Give the ability to the script to link custom function to the "delete_item" event.

  - ITEM_EVENTS:EDIT_ITEM > Give the ability to the script to link custom function to the "edit_item" event.

  - ITEM_EVENTS:SELECT_ITEM > Give the ability to the script to link custom function to the "select_item" event.

Medium-Level Permissions
------------------------

- LIMITED_FILE > Give the ability to the script to create, edit, remove, read file that he created himself for script, and for files that are found in the plugin folder for plugin.

  - LIMITED_FILE:READ > Give the ability to the script to read file that he created himself for script, and for files that are found in the plugin folder for plugin.

  - LIMITED_FILE:REMOVE > Give the ability to the script to remove file that he created himself for script, and for files that are found in the plugin folder for plugin.

  - LIMITED_FILE:EDIT > Give the ability to the script to edit file that he created himself for script, and for files that are found in the plugin folder for plugin.
  - LIMITED_FILE:CREATE > Give the ability to the script to create file for script, and for plugin, only in is own plugin folder.
