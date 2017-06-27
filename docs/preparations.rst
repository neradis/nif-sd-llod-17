==============
 Preparations
==============

Suitable Text Editor
====================

You should have a text editor set up which offers syntax-highlighting for Turtle
(an RDF serialisation format) and (optionally) for SPARQL queries.

Several more powerful editor (e.g. `Emacs`_, `Vim`_, `Notepad++`_) either
support support for these syntaxes out of the box or there are appropriate
community extensions. Thus, if you are experienced in their usage, setting up
your favorite of these editors for Turtle and SPARQL might be your best option.

For all users with no prior experience with the aforementioned editors, we
recommend installing and setting up Atom for this session. Installers for the
recent version for all common platform are `available at GitHub`__. After
installation of Atom, you can install the packages `language-rdf`_ and
`language-sparql`_ directly from within the Editor itself, using the
`Settings`_. If you prefer the command line way, just type: :command:`apm
install language-rdf` and :command:`apm install language-sparql`

__ AtomRelease_


Java 8 JRE
==========

Most tools that will be used in the session require the Java Runtime Environment
(or Java Development Kit) Version 8. For recent Linux distributions, a Java 8
JRE should be available in the official repositories. If you are on Windows or
Mac and do not have Java 8 set up already, please obtain it `from Oracle`__.

__ OracleJava8_

Please also ensure that the directory with the Java executables has been added
to your :envvar:`$PATH`. To verify that :envvar:`$PATH` is set correctly, enter
``java -version`` into a command line prompt. The output should contain
``version "1.8.0`` as a substring.


Notes on Command Prompt Usage (only relevant on Windows)
========================================================

We will use the command prompt regularly in this session. For the sake of
simplicity, the rest of the documentation will give the command examples
generally with the command names for BASH, the default command prompt on
(almost) all Linux versions.

Current versions of Windows mostly ship with the PowerShell, which has aliases
for all the common BASH commands occurring in this tutorial to their Windows
counterparts, thus, the commands should be executable in a PowerShell session
without alterations. If you use the traditional Windows Command Prompt, some
command names and or options will have to be adjusted by you
(e.g. ``dir`` instead of ``ls``). Alternatively, Babun_ can be
used.


.. _AtomRelease:  https://github.com/atom/atom/releases/tag/v1.17.2
.. _Emacs: https://www.gnu.org/software/emacs/manual/
.. _Vim: https://vim.sourceforge.io/docs.php
.. _Notepad++: https://notepad-plus-plus.org/
.. _Settings: http://flight-manual.atom.io/using-atom/sections/atom-packages/
.. _language-rdf: https://atom.io/packages/language-rdf
.. _language-sparql: https://atom.io/packages/language-sparql
.. _OracleJava8: http://www.oracle.com/technetwork/java/javase/downloads/jre8-downloads-2133155.html
.. _Babun: http://babun.github.io/
