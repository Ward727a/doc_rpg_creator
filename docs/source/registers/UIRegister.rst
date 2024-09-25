UI Register
==============

The UI Register is the area where all UI created by LUA can be found. 
As a majority of UI in the software is created by LUA, you can get all of the UI with this object.

You can even replace them by your own UI by "overriding" the key of the UI.

Each UI has 1 unique key.

LUA Methods
-------------

.. table::
   :widths: auto

   +-----------------------------------------------------------------------------+-----------------------------------------------------------------------------------+-----------+
   | |bool|                                                                      | :ref:`has_ui<class_Registers_UI_Method_has_ui>`                                   | ``0``     |
   +-----------------------------------------------------------------------------+-----------------------------------------------------------------------------------+-----------+

LUA Method Descriptions
-------------------
.. class_Registers_UI_Method_has_ui:
|bool| has_ui(\UI_Key\: String\)
This method will check if the UI key given exist or not.

.. rst-class:: classref-item-separator

----
