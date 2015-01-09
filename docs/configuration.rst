Configuration
=============

You can configure djed.static via your ini-file::

    [app:myapp]
    djed.static.components_name = lib
    ...

To understand the ini-setting options, let's take a look at the URL structure
that is generated by BowerStatic::

    /bowerstatic/components/jquery/2.1.1/dist/jquery.js

Or for local components::

    /bowerstatic/local/mycomponent/1.0.0/mycomponent.js

The setting options allow you to change the first two parts of the URLs:

``djed.static.publisher_signature``
    The first part of the components and local URLs.

    default: ``bowerstatic``

``djed.static.components_name``
    The second part of the components URLs.

    default: ``components``

``djed.static.local_components_name``
    The second part of the local URLs.

    default: ``local``