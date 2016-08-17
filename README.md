USOS extensions to the ELMO format
==================================

The [EMREX response ELMO XML schema][elmo-spec] allows developers to attach
custom elements to their ELMO files. Our NCP implementation will use these
extensions in order to provide some additional functionality currently needed
for successful deployment of EMREX in Poland.


Extra NCP parameters
--------------------

WRTODO


Extra ELMO extensions
---------------------

In order for the clients to make use of the extra NCP parameters described in
the previous section, our NCP will include additional elements in the
produced ELMO files. These elements are described in the attached [schema.xsd]
(schema.xsd) file.


[elmo-spec]: https://github.com/emrex-eu/elmo-schemas
