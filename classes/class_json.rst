.. Generated automatically by doc/tools/makerst.py in Godot's source tree.
.. DO NOT EDIT THIS FILE, but the JSON.xml source instead.
.. The source is found in doc/classes or modules/<name>/doc_classes.

.. _class_JSON:

JSON
====

**Inherits:** :ref:`Object<class_object>`

**Category:** Core

Brief Description
-----------------

Helper class for parsing JSON data.

Member Functions
----------------

+------------------------------------------------+----------------------------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`JSONParseResult<class_jsonparseresult>`  | :ref:`parse<class_JSON_parse>` **(** :ref:`String<class_string>` json **)**                                                                                    |
+------------------------------------------------+----------------------------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`String<class_string>`                    | :ref:`print<class_JSON_print>` **(** :ref:`Variant<class_variant>` value, :ref:`String<class_string>` indent="", :ref:`bool<class_bool>` sort_keys=false **)** |
+------------------------------------------------+----------------------------------------------------------------------------------------------------------------------------------------------------------------+

Description
-----------

Helper class for parsing JSON data. For usage example and other important hints, see :ref:`JSONParseResult<class_jsonparseresult>`.

Member Function Description
---------------------------

.. _class_JSON_parse:

- :ref:`JSONParseResult<class_jsonparseresult>` **parse** **(** :ref:`String<class_string>` json **)**

Parses a JSON encoded string and returns a :ref:`JSONParseResult<class_jsonparseresult>` containing the result.

.. _class_JSON_print:

- :ref:`String<class_string>` **print** **(** :ref:`Variant<class_variant>` value, :ref:`String<class_string>` indent="", :ref:`bool<class_bool>` sort_keys=false **)**

Converts a Variant var to JSON text and returns the result. Useful for serializing data to store or send over the network.


