USOS extensions to EMREX
========================

Polish NCP implementations will use some unofficial extensions in order to
provide additional functionality currently needed for successful deployment of
EMREX in Poland. This document describes these extensions publicly, so that all
developers (both external and internal) can easily know what's going on.

Extra NCP parameters
--------------------

Apart from the regular parameters, our NCP takes some additional ones. All of
them are **optional**, and the default values correspond with the default
behavior imposed by the official EMREX NCP specifications.


### `allowToPickCourses`

Boolean (`true` or `false`). **Default is true.**

When this is set to `false`, then students won't have the option to choose
which courses they want to export. If export succeeds then all courses will be
exported. (Note, that the definition of "all" is still dependant on the values
of the other parameters.)


### `allowNotPassedCourses`

Boolean (`true` or `false`). **Default is false.**

When this is set to `true`, then all courses will displayed to the student,
including the *failed* courses, and the courses which he has not finished yet.


ELMO file extensions
--------------------

[EMREX ELMO schema][elmo-spec] allows developers to attach custom `<extension>`
elements to their ELMO files. Our NCP implementation will make use of these
extensions:

 * See attached [schema.xsd](schema.xsd) file for details.


[elmo-spec]: https://github.com/emrex-eu/elmo-schemas
