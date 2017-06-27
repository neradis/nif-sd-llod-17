=======
 Tools
=======

.. _jena-cmds:

Apache Jena Command Line Tools
==============================

Jenas command line tools are a collection of Shell scripts/Batch scripts that
allow to access functionalities of that RDF/OWL programming library without
composing Java programs. For the excercises proposed, usage will probably be
limited to the tool that reads Turtle RDF documents to either validate them
syntactically or to convert them to another RDF serialisation
format. (``turtle``/ ``turtle.bat``).


.. _fuseki:

Fuseki SPARQL Server
====================

Fuseki allows to query and update configured RDF datasets using SPARQL
queries. It also offers a browser-based application to formulate and execute
SPARQL queries with syntax highlighting and hints for syntactic error in entered
queries.

You find a copy of Fuseki pre-configured for the excercises in
:file:`tools/fuseki`. To start it, oben a new terminal window, navigate to that
directory and run the start script ``./fuseki-server`` (Linux/Mac) or
``.\fuseki-server.bat`` (Windows). The command prompt will remain occupied by
the server process during execution and log messages about the initlization
process, received queries etc. will be printed. To terminate the server process,
send ``SIGINT`` by pressing **CTRL +C** in the terminal with the server process
running.



Once Fuseki has been started, you can visit
:samp:`http://localhost:3030/dataset.html` to access the graphical SPARQL user
interface. Ensure that the appropriate dataset for the excercise you intend to
tackle is selected in the *'Dataset'* drow-down menu at the top. (``/wilde`` for
Excercise A, ``/brown`` for Exercise B).


.. _lodlive:

LodLive Web of Data Browser
===========================

LodLive is a Javascript-based browser application that allows stepwise
exploration of RDF knowledge graphs. A copy of LodLive slightly modified and
pre-configured for this session is located in the :file:`tools/lodlive`
directory.

To lauch, open the :file:`app_en.html` start page in that directory in your
browser. When invoking this HTML document without additional query parameters in
the URL, you will be presented with a start screen. The boxes in the lower row
in light green represent the configured local datasets. With the contained
dropdown menus you can select example resources to start a browsing session. If
you already know a specific resource IRI you would like to use as starting
point, you can either enter it in the blue box on the start screen or add it to
the URL presented in the navigation bar of your browser:

    :samp:`file://{$MATERIALS_ROOT}/tools/lodlive/app_en.html?{$RESOURCE_IRI}`

When after selecting your entry resource, you will see the actual graph
exploration view with the representation of the selected resource as first
circle in the center of the viewport. Although usage for further exploration is
quite intutive, please consider opening and skimming the in-app explanation
offered by buttons on the left side of the viewport.
          
          
.. note:: LodLive retrieves the statements to describe and visualise resources
   from the local :ref:`fuseki`, so please ensure that it is up and running
   before using LodLive.
