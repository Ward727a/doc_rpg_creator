UI Register
==============

.. warning::

   This page is still under-construction!

   Some information could be missing.

The UI Register is the area where all UI
created by LUA can be found.
As a majority of UI in the software is created by
LUA, you can get all of the UI with this object.

You can even replace them by your own UI by "overriding" the key of the UI.

Each UI has 1 unique key.


.. note::

   To use those methods you need to ask for permission: `REGISTERS` or `REGISTERS:UI`!


LUA Methods
-------------


.. table::
   :widths: auto

   +-----------+---------------------------------------------------------------------+
   | *bool*    | :ref:`has_ui<class_Registers_UI_Method_has_ui>`\ (\String)          |
   +-----------+---------------------------------------------------------------------+
   | *bool*    | :ref:`add_ui<class_Registers_UI_Method_add_ui>`\ (\String, Control) |
   +-----------+---------------------------------------------------------------------+
   | *bool*    | :ref:`set_ui<class_Registers_UI_Method_set_ui>`\ (\String, Control) |
   +-----------+---------------------------------------------------------------------+
   | *Control* | :ref:`get_ui<class_Registers_UI_Method_get_ui>`\ (\String)          |
   +-----------+---------------------------------------------------------------------+
   | *Array*   | :ref:`get_ui_list<class_Registers_UI_Method_get_ui_list>`\ (\ )     |
   +-----------+---------------------------------------------------------------------+
   | *bool*    | :ref:`remove_ui<class_Registers_UI_Method_remove_ui>`\ (\String)    |
   +-----------+---------------------------------------------------------------------+

.. rst-class:: classref-descriptions-group

LUA Method Descriptions
-----------------------

.. _class_Registers_UI_Method_has_ui:

.. rst-class:: classref-method

*bool* **has_ui**\ (\UI_Key\: *String*\)

This method will check if the UI key given exist or not.

If the key doesn't exist, this method will
return false, and will return true if it exist.

.. rst-class:: classref-item-separator

----

.. _class_Registers_UI_Method_add_ui:

.. rst-class:: classref-method

*bool* **add_ui**\ (\UI_Key\: *String*, UI_Node\: *Control*\)

This method will add an UI to the register with the specified key.

If the key already exist, it will return false and will not add the UI.

For replacing UI that already exist, check:
:ref:`set_ui<class_Registers_UI_Method_set_ui>` method!

.. rst-class:: classref-item-separator

----

.. _class_Registers_UI_Method_set_ui:

.. rst-class:: classref-method

*bool* **set_ui**\ (\UI_Key\: *String*, Control\: *Control*\)

This method will add or replace an UI to the register with the specified key.

If the key already exist, it will be replaced by the new node given.

.. rst-class:: classref-item-separator

----

.. _class_Registers_UI_Method_get_ui:

.. rst-class:: classref-method

*Control* **get_ui**\ (\UI_Key\: *String*\)

This method will return the node of the UI if the specified key can be found.

If not, it will return "null" so be sure to check if the UI_key exist or not!

.. rst-class:: classref-item-separator

----

.. _class_Registers_UI_Method_get_ui_list:

.. rst-class:: classref-method

*Array* **get_ui_list**\ (\)

This method will return a list of all UI_Key that are in the UI Register.

.. rst-class:: classref-item-separator

----

.. _class_Registers_UI_Method_remove_ui:

.. rst-class:: classref-method

*bool* **remove_ui**\ (\UI_Key\: *String*)

This method will try to remove an UI with the specified UI Key.

It return true if the UI as been removed with success, false otherwise.

