.. Copyright (c) 2007-2016 UShareSoft, All rights reserved

.. _partitionTableLogicalVolume-get:

partitionTableLogicalVolume_get
-------------------------------

.. function:: GET users/{uid}/appliances/{aid}/installProfile/{ipid}/pt/{ptid}/volumes/{vid}

.. sidebar:: Summary

	* Method: ``GET``
	* Response Code: ``200 / 304``
	* Response Formats: ``application/xml`` ``application/json``
	* Since: ``UForge 2.1``

Retrieves the information of a logical volume.

Security Summary
~~~~~~~~~~~~~~~~

* Requires Authentication: ``true``
* Entitlements Required: ``appliance_create``

URI Parameters
~~~~~~~~~~~~~~

* ``vid`` (required): the id of the :ref:`logicalvolume-object`
* ``uid`` (required): the id of the :ref:`user-object` that has created the appliance
* ``ptid`` (required): the id of the :ref:`partitiontable-object`
* ``aid`` (required): the id of the :ref:`appliance-object`

HTTP Request Body Parameters
~~~~~~~~~~~~~~~~~~~~~~~~~~~~

None

Example Request
~~~~~~~~~~~~~~~

.. code-block:: bash

	curl "users/{uid}/appliances/{aid}/installProfile/{ipid}/pt/{ptid}/volumes/{vid}" -X GET \
	-u USER_LOGIN:PASSWORD -H "Accept: application/xml"

.. seealso::

	 * :ref:`appliancepartitiontabledisk-api-resources`
	 * :ref:`appliancepartitiontablediskpartition-api-resources`
	 * :ref:`appliancepartitiontablelogicalgroup-api-resources`
	 * :ref:`partitiontable-object`
	 * :ref:`appliance-object`
	 * :ref:`logicalvolume-object`
	 * :ref:`partitionTableLogicalVolume-create`
	 * :ref:`partitionTableLogicalVolume-getAll`
	 * :ref:`partitionTableLogicalVolume-delete`
	 * :ref:`partitionTableLogicalVolume-deleteAll`
	 * :ref:`partitionTableLogicalVolume-update`