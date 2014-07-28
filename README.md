ansible-javax
=============

An Ansible module for executing an arbitrary java class or jar

Options:

- classpath

A list of file system paths the JVM should search to find any dependencies. The module will take the list and properly concatenate the list of values. The equivalent of the `-classpath' or `-cp' commandline option.

- executable

Path to java JVM to use. If not supplied, the normal mechanism for resolving binary paths will be used.

- init_heap_size

Sets initial Java heap size for the application. Equivalent of the `-Xms' 'non-stndard' commandline option.

- jar

The JAR file that contains the Java class you want to run. Required if the `javaclass' option is omitted.

- java_args

Specify a list of strings to be passed as parameters to the java application.

- java_opts

Specify additional java options not supported by this module by passing in a list of strings.

- javaclass

The main Java class to run. Required if the `jar' option is omitted.

- max_heap_size

Sets maximum Java heap size for the application. Equivalent of the `-Xmx' 'non-stndard' commandline option.

- properties

A dict of key value pairs representing system properties to pass the java application being run. This is the equivalent of the `-D' commandline option.

- thread_stack

Sets java thread stack size for the application. Equivalent of the `-Xss' 'non-stndard' commandline option.
