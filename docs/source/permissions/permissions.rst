Permission System
=================

.. warning::

  This page is still under-construction!

  Some information could be missing.

The permission system was created to allow the user
of custom script to control what a script can do.

When a developer create a custom script / plugin, they
need to ask for permissions before using a lot of methods,
if the script try to access a method that was not asked before
by a permission, the script will not work as the software didn't
give the permission to do it.

There is 3 levels of permission:

- Low-level: Those permissions will just show a message
  box to the user where the user can allow all, some or none.

- Medium-level: Those permissions are more powerfull
  than low-level, so the user will get a warning message
  before accepting the permission.

- High-level: Those permissions are **VERY** powerfull,
  they can remove file, create new file, access internet,...
  So the user will get a warning message where he need to wait 5
  seconds and write a text in a box before having the right to accept.

If a user refuse to give the permission to a script, the
script can ask again **one** time only, after that, the script
will not be able to ask anymore and the user will need to allow it
manually in the software settings.

------------------------------------

Below will be a list of all permissions that can be asked by a script.

For each category of permission, there will be a list of all
permissions that can be asked by a script.

For example, if we take the "UI" category, and we want to use
the "COMPONENTS" permission, we will need to ask for the
"UI:COMPONENTS" permission.

------------------------------------

Low-Level Permissions
---------------------

UI
###########

Give the ability to the script to create custom UI nodes.

.. table::
  :widths: auto

  +--------------+----------------------------------------------------+
  | Permission   | Description                                        |
  +==============+====================================================+
  | COMPONENTS   | Give the ability to the script to create components|
  |              | of an UI. (Button, Label, Image, etc...)           |
  +--------------+----------------------------------------------------+
  | ADD_UI       | Give the ability to the script to add an UI to the |
  |              | software by his key. This will do nothing if the   |
  |              | key already exist.                                 |
  +--------------+----------------------------------------------------+
  | REMOVE_UI    | Give the ability to the script to remove an UI from|
  |              | the software by his key.                           |
  +--------------+----------------------------------------------------+
  | SET_UI       | Give the ability to the script to set an UI by his |
  |              | key, this will replace the UI if the key already   |
  |              | exist.                                             |
  +--------------+----------------------------------------------------+
  | GET_UI       | Give the ability to the script to get an UI by his |
  |              | key.                                               |
  +--------------+----------------------------------------------------+
  | GET_UI_LIST  | Give the ability to the script to get the list of  |
  |              | all UI.                                            |
  +--------------+----------------------------------------------------+
  | HAS_UI       | Give the ability to the script to check if an UI   |
  |              | exist or not.                                      |
  +--------------+----------------------------------------------------+

ITEM_PARAMETERS
###############

Give the ability to the script to create custom item parameters.

.. table::
  :widths: auto

  +------------------------------+----------------------------------------------------+
  | Permission                   | Description                                        |
  +==============================+====================================================+
  | ADD_PARAMETER                | Give the ability to the script to add a new        |
  |                              | parameter to the software.                         |
  +------------------------------+----------------------------------------------------+
  | REMOVE_PARAMETER             | Give the ability to the script to remove a         |
  |                              | parameter from the software.                       |
  +------------------------------+----------------------------------------------------+
  | HAS_PARAMETER                | Give the ability to the script to check if a       |
  |                              | parameter exist or not.                            |
  +------------------------------+----------------------------------------------------+
  | SET_PARAMETER                | Give the ability to the script to set a parameter  |
  |                              | by his key.                                        |
  +------------------------------+----------------------------------------------------+
  | SET_PARAMETERS               | Give the ability to the script to set mutiple      |
  |                              | parameters at once.                                |
  +------------------------------+----------------------------------------------------+
  | GET_PARAMETER                | Give the ability to the script to get a parameter  |
  |                              | by his key.                                        |
  +------------------------------+----------------------------------------------------+
  | GET_COPY_PARAMETER           | Give the ability to the script to get a copy       |
  |                              | of a parameter by his key.                         |
  +------------------------------+----------------------------------------------------+
  | ADD_CATEGORY                 | Give the ability to the script to add a new        |
  |                              | category to the software.                          |
  +------------------------------+----------------------------------------------------+
  | REMOVE_CATEGORY              | Give the ability to the script to remove a         |
  |                              | category from the software.                        |
  +------------------------------+----------------------------------------------------+
  | GET_CATEGORIES               | Give the ability to the script to get all          |
  |                              | categories that are present in the software.       |
  +------------------------------+----------------------------------------------------+
  | HAS_CATEGORY                 | Give the ability to the script to check if a       |
  |                              | category exist or not.                             |
  +------------------------------+----------------------------------------------------+
  | GET_CATEGORY_PARAMETERS_KEYS | Give the ability to the script to get all          |
  |                              | parameters keys of a category.                     |
  +------------------------------+----------------------------------------------------+


ITEM_EVENTS
###########

Give the ability to the script to link custom function to item event.

.. table::
  :name: item_events
  :widths: auto

  +----------------+----------------------------------------------------+
  | Permission     | Description                                        |
  +================+====================================================+
  | NEW_ITEM       | Give the ability to the script to link custom      |
  |                | function to the "new_item" event.                  |
  +----------------+----------------------------------------------------+
  | DELETE_ITEM    | Give the ability to the script to link custom      |
  |                | function to the "delete_item" event.               |
  +----------------+----------------------------------------------------+
  | EDIT_ITEM      | Give the ability to the script to link custom      |
  |                | function to the "edit_item" event.                 |
  +----------------+----------------------------------------------------+
  | SELECT_ITEM    | Give the ability to the script to link custom      |
  |                | function to the "select_item" event.               |
  +----------------+----------------------------------------------------+

Medium-Level Permissions
------------------------

- LIMITED_FILE > Give the ability to the script to create, edit,
  remove, read file that he created himself for script, and for files
  that are found in the plugin folder for plugin.

  - LIMITED_FILE:READ > Give the ability to the script to read file
    that he created himself for script, and for files that are found
    in the plugin folder for plugin.

  - LIMITED_FILE:REMOVE > Give the ability to the script to remove
    file that he created himself for script, and for files that are
    found in the plugin folder for plugin.

  - LIMITED_FILE:EDIT > Give the ability to the script to edit file
    that he created himself for script, and for files that are found
    in the plugin folder for plugin.

  - LIMITED_FILE:CREATE > Give the ability to the script to create
    file for script, and for plugin, only in is own plugin folder.
