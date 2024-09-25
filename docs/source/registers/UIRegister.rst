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

   +-----------------------------------------------------------------------------+-----------------------------------------------------------------------------------+
   | *bool*                                                                      | :ref:`has_ui<class_Registers_UI_Method_has_ui>`\ (\String)                        |
   +-----------------------------------------------------------------------------+-----------------------------------------------------------------------------------+

.. rst-class:: classref-descriptions-group

LUA Method Descriptions
-------------------
.. _class_Registers_UI_Method_has_ui:

.. rst-class:: classref-method

*bool* **has_ui**\ (\UI_Key\: *String*\)

This method will check if the UI key given exist or not.

If the key doesn't exist, this method will return false, and will return true if it exist.

.. rst-class:: classref-item-separator

----
