.. include:: /Includes.rst.txt

.. _columns-inline-properties-fshowNewRecordLink:

=================
showNewRecordLink
=================

.. confval:: showNewRecordLink

   :type: boolean
   :Scope: Display
   :Default: true

   Disables the :guilabel:`New record` link in TCA `inline` elements without
   without simultaneously also disabling either the
   :guilabel:`+` button in each inline records' header (using
   :ref:`['appearance']['enabledControls']['new']
   <columns-inline-properties-appearance>`) or all other
   "level links" (using :ref:`['appearance']['levelLinksPosition'] = 'none'
   <columns-inline-properties-appearance>`).

Example
=======

Disable the :guilabel:`New record` button:

.. code-block:: php

    'inlineField' => [
        'label' => 'Inline without New record link',
        'config' => [
            'type' => 'inline',
            'appearance' => [
                'showNewRecordLink' => false,
            ],
        ],
    ],
