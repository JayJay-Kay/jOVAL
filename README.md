Joval&trade; Open-source Data Model
=============

jOVAL is an open-source JAXB data model for the SCAP specification languages, including:
* XCCDF
* OVAL
* OCIL
* ARF
* AI
* CPE
* CVE

Having an open-source JAXB data model for the SCAP specifications makes it possible for multiple parties to write Java programs that are compatible with one-another without requiring the XML formats to be marshalled and unmarshalled. Additionally, jOVAL also includes schema registration resources and a data-model extension mechanism that makes it possible for jOVAL customers to implement their own OVAL test types and use them with jOVAL's OVAL processing engine. For more information on the extension mechanism, see [scap-extensions](scap-extensions).

To encourage adoption by third-parties, the jOVAL project is now licensed using the LGPL.

For more information, visit <http://joval.org>.

Building jOVAL
=============

The project can be built using GNU make; simply run 'make' from the project's root directory. Before doing so, however, you must:

1) set a JAVA_HOME environment variable set that points to the base directory of a JDK. The project requires Java 6 or later. When using Java 6, you must also specify a JAXB_HOME environment variable specifying the install path of a compatible JAXB_RI (version 2.2.4 or later).
2) run ```git submodule init``` and ```git submodule update```. This will fetch the OVAL-Community/OVAL git repository, which is the official current version of the OVAL language. The submodule is installed at 3rd-party/OVAL.

&nbsp;
=============

Copyright (c) 2011-2020, JovalCM.com.  All rights reserved.
