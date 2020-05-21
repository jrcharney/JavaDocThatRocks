# All the Packages!

This document lists all the packages in Java SE and JDK as of **JDK 14**.

For things like JUnit or other products, look on the [Index](index.md) page.

> **Note**: Some of these packages may be deprecated. Deprecated classes won't be documented but they will be listed.

> **TODO**: Add when they were added/removed. Generally given by the `@since` or `@depricated` annotations.

## All the Packages!

> TODO: Map out the indirect exports

### Sun Microsystems

| Module | Package | Description |
| :--- | :--- | :--- |
| [`jdk.jartool`](jdk.jartool.md) | ~~`com.sun.jarsigner`~~ | ~~This package comprises the interfaces and classes used to define the signing mechanism used by the `jarsigner` tool.~~ **Deprecated.**
| [`jdk.accessibility`](jdk.accessibility.md) | [`com.sun.java.accessibility.util`](com.sun.java.accessibility.util.md) | Provides a collection of interfaces and classes that compose the Java Accessibility Utilities.
| [`jdk.jdi`](jdk.jdi.md) | [`com.sun.jdi`](com.sun.jdi.md) | This is the core package of the Java Debug Interface (JDI), it defines mirrors for values, types, and the target VirtualMachine itself - as well bootstrapping facilities.
| [`jdk.jdi`](jdk.jdi.md) | [`com.sun.jdi.connect`](com.sun.jdi.connect.md) | This package defines connections between the virtual machine using the JDI and the target virtual machine.
| [`jdk.jdi`](jdk.jdi.md) | [`com.sun.jdi.connect.spi`](com.sun.jdi.connect.spi.md) | This package comprises the interfaces and classes used to develop new [**`TransportService`**](com.sun.jdi.connect.spi.md "class in com.sun.jdi.connect.spi") implementations.
| [`jdk.jdi`](jdk.jdi.md) | [`com.sun.jdi.event`](com.sun.jdi.event.md) | This package defines JDI events and event processing.
| [`jdk.jdi`](jdk.jdi.md) | [`com.sun.jdi.request`](com.sun.jdi.request.md) | This package is used to request that a JDI event be sent under specified conditions.
| [`jdk.management`](jdk.management.md) | [`com.sun.management`](com.sun.management.md) | This package contains the JDK's extension to the standard implementation of the [`java.lang.management`](java.lang.management.md) API and also defines the management interface for some other components of the platform.
| [`jdk.httpserver`](jdk.httpserver.md) | [`com.sun.net.httpserver`](com.sun.net.httpserver.md) | Provides a simple high-level Http server API, which can be used to build embedded HTTP servers.
| [`jdk.httpserver`](jdk.httpserver.md) | [`com.sun.net.httpserver.spi`](com.sun.net.httpserver.spi.md) | Provides a pluggable service provider interface, which allows the HTTP server implementation to be replaced with other implementations.
| [`jdk.sctp`](jdk.sctp.md) | [`com.sun.nio.sctp`](com.sun.nio.sctp.md) | A Java API for Stream Control Transport Protocol.
| [`jdk.security.auth`](jdk.security.auth.md) | [`com.sun.security.auth`](com.sun.security.auth.md) | Provides implementations of [**`Principal`**](java.security.md "interface in java.security").
| [`jdk.security.auth`](jdk.security.auth.md) | [`com.sun.security.auth.callback`](com.sun.security.auth.callback.md) | Provides an implementation of [**`CallbackHandler`**](javax.security.auth.callback.md "interface in javax.security.auth.callback").
| [`jdk.security.auth`](jdk.security.auth.md) | [`com.sun.security.auth.login`](com.sun.security.auth.login.md) | Provides an implementation of [**`Configuration`**](javax.security.auth.login.md "class in javax.security.auth.login").
| [`jdk.security.auth`](jdk.security.auth.md) | [`com.sun.security.auth.module`](com.sun.security.auth.module.md) | Provides implementations of [**`LoginModule`**](javax.security.auth.spi.md "interface in javax.security.auth.spi").
| [`jdk.security.jgss`](jdk.security.jgss.md) | [`com.sun.security.jgss`](com.sun.security.jgss.md) | This package defines classes and interfaces for the JDK extensions to the GSS-API.
| [`jdk.compiler`](jdk.compiler.md) | [`com.sun.source.doctree`](com.sun.source.doctree.md) | Provides interfaces to represent documentation comments as abstract syntax trees (AST).
| [`jdk.compiler`](jdk.compiler.md) | [`com.sun.source.tree`](com.sun.source.tree.md) | Provides interfaces to represent source code as abstract syntax trees (AST).
| [`jdk.compiler`](jdk.compiler.md) | [`com.sun.source.util`](com.sun.source.util.md) | Provides utilities for operations on abstract syntax trees (AST).
| [`jdk.attach`](jdk.attach.md) | [`com.sun.tools.attach`](com.sun.tools.attach.md) | Provides the API to attach to a Java™ virtual machine.
| [`jdk.attach`](jdk.attach.md) | [`com.sun.tools.attach.spi`](com.sun.tools.attach.spi.md) | Only developers who are defining new attach providers should need to make direct use of this package.
| [`jdk.compiler`](jdk.compiler.md) | [`com.sun.tools.javac`](com.sun.tools.javac.md) | This package provides a legacy entry point for the `javac` tool.
| [`jdk.jconsole`](jdk.jconsole.md) | [`com.sun.tools.jconsole`](com.sun.tools.jconsole.md) | This package contains the JConsole API.

### Java

| Module | Package | Description |
| :--- | :--- | :--- |
| [`java.desktop`](java.desktop.md) | ~~`java.applet`~~ | ~~Provides the classes necessary to create an applet and the classes an applet uses to communicate with its applet context.~~ **Deprecated.**
| [`java.desktop`](java.desktop.md) | [`java.awt`](java.awt.md) | Contains all of the classes for creating user interfaces and for painting graphics and images.
| [`java.desktop`](java.desktop.md) | [`java.awt.color`](java.awt.color.md) | Provides classes for color spaces.
| [`java.datatransfer`](java.datatransfer.md) | [`java.awt.datatransfer`](java.awt.datatransfer.md) | Provides interfaces and classes for transferring data between and within applications.
| [`java.desktop`](java.desktop.md) | [`java.awt.desktop`](java.awt.desktop.md) | Provides interfaces and classes for interaction with various desktop capabilities.
| [`java.desktop`](java.desktop.md) | [`java.awt.dnd`](java.awt.dnd.md) | Drag and Drop is a direct manipulation gesture found in many Graphical User Interface systems that provides a mechanism to transfer information between two entities logically associated with presentation elements in the GUI.
| [`java.desktop`](java.desktop.md) | [`java.awt.event`](java.awt.event.md) | Provides interfaces and classes for dealing with different types of events fired by AWT components.
| [`java.desktop`](java.desktop.md) | [`java.awt.font`](java.awt.font.md) | Provides classes and interface relating to fonts.
| [`java.desktop`](java.desktop.md) | [`java.awt.geom`](java.awt.geom.md) | Provides the Java 2D classes for defining and performing operations on objects related to two-dimensional geometry.
| [`java.desktop`](java.desktop.md) | [`java.awt.im`](java.awt.im.md) | Provides classes and interfaces for the input method framework.
| [`java.desktop`](java.desktop.md) | [`java.awt.im.spi`](java.awt.im.spi.md) | Provides interfaces that enable the development of input methods that can be used with any Java runtime environment.
| [`java.desktop`](java.desktop.md) | [`java.awt.image`](java.awt.image.md) | Provides classes for creating and modifying images.
| [`java.desktop`](java.desktop.md) | [`java.awt.image.renderable`](java.awt.image.renderable.md) | Provides classes and interfaces for producing rendering-independent images.
| [`java.desktop`](java.desktop.md) | [`java.awt.print`](java.awt.print.md) | Provides classes and interfaces for a general printing API.
| [`java.desktop`](java.desktop.md) | [`java.beans`](java.beans.md) | Contains classes related to developing *beans* -- components based on the JavaBeans™ architecture.
| [`java.desktop`](java.desktop.md) | [`java.beans.beancontext`](java.beans.beancontext.md) | Provides classes and interfaces relating to bean context.
| [`java.base`](java.base.md) | [**`java.io`**](java.io.md) | Provides for system input and output through data streams, serialization and the file system.
| [`java.base`](java.base.md) | [**`java.lang`**](java.lang.md) | Provides classes that are fundamental to the design of the Java programming language.
| [`java.base`](java.base.md) | [`java.lang.annotation`](java.lang.annotation.md) | Provides library support for the Java programming language annotation facility.
| [`java.base`](java.base.md) | [`java.lang.constant`](java.lang.constant.md) | Classes and interfaces to represent *nominal descriptors* for run-time entities such as classes or method handles, and classfile entities such as constant pool entries or `invokedynamic` call sites.
| [`java.lang.instrument`](java.lang.instrument.md) | [`java.lang.instrument`](java.lang.instrument.md) | Provides services that allow Java programming language agents to instrument programs running on the JVM.
| [`java.base`](java.base.md) | [`java.lang.invoke`](java.lang.invoke.md) | The `java.lang.invoke` package provides low-level primitives for interacting with the Java Virtual Machine.
| [`java.management`](java.management.md) | [`java.lang.management`](java.lang.management.md) | Provides the management interfaces for monitoring and management of the Java virtual machine and other components in the Java runtime.
| [`java.base`](java.base.md) | [`java.lang.module`](java.lang.module.md) | Classes to support module descriptors and creating configurations of modules by means of resolution and service binding.
| [`java.base`](java.base.md) | [`java.lang.ref`](java.lang.ref.md) | Provides reference-object classes, which support a limited degree of interaction with the garbage collector.
| [`java.base`](java.base.md) | [`java.lang.reflect`](java.lang.reflect.md) | Provides classes and interfaces for obtaining reflective information about classes and objects.
| [`java.base`](java.base.md) | [`java.lang.runtime`](java.lang.runtime.md) | The `java.lang.runtime` package provides low-level runtime support for the Java language.
| [`java.base`](java.base.md) | [`java.math`](java.math.md) | Provides classes for performing arbitrary-precision integer arithmetic (`BigInteger`) and arbitrary-precision decimal arithmetic (`BigDecimal`).
| [`java.base`](java.base.md) | [`java.net`](java.net.md) | Provides the classes for implementing networking applications.
| [`java.net.http`](java.net.http.md) | [`java.net.http`](java.net.http.md) | HTTP Client and WebSocket APIs
| [`java.base`](java.base.md) | [`java.net.spi`](java.net.spi.md) | Service-provider classes for the [`java.net`](java.net.md) package.
| [`java.base`](java.base.md) | [`java.nio`](java.nio.md) | Defines buffers, which are containers for data, and provides an overview of the other NIO packages.
| [`java.base`](java.base.md) | [`java.nio.channels`](java.nio.channels.md) | Defines channels, which represent connections to entities that are capable of performing I/O operations, such as files and sockets; defines selectors, for multiplexed, non-blocking I/O operations.
| [`java.base`](java.base.md) | [`java.nio.channels.spi`](java.nio.channels.spi.md) | Service-provider classes for the [`java.nio.channels`](java.nio.channels.md) package.
| [`java.base`](java.base.md) | [`java.nio.charset`](java.nio.charset.md) | Defines charsets, decoders, and encoders, for translating between bytes and Unicode characters.
| [`java.base`](java.base.md) | [`java.nio.charset.spi`](java.nio.charset.spi.md) | Service-provider classes for the [`java.nio.charset`](java.nio.charset.md) package.
| [`java.base`](java.base.md) | [`java.nio.file`](java.nio.file.md) | Defines interfaces and classes for the Java virtual machine to access files, file attributes, and file systems.
| [`java.base`](java.base.md) | [`java.nio.file.attribute`](java.nio.file.attribute.md) | Interfaces and classes providing access to file and file system attributes.
| [`java.base`](java.base.md) | [`java.nio.file.spi`](java.nio.file.spi.md) | Service-provider classes for the [`java.nio.file`](java.nio.file.md) package.
| [`java.rmi`](java.rmi.md) | [`java.rmi`](java.rmi.md) | Provides the RMI package.
| [`java.rmi`](java.rmi.md) | [`java.rmi.activation`](java.rmi.activation.md) | Provides support for RMI Object Activation.
| [`java.rmi`](java.rmi.md) | [`java.rmi.dgc`](java.rmi.dgc.md) | Provides classes and interface for RMI distributed garbage-collection (DGC).
| [`java.rmi`](java.rmi.md) | [`java.rmi.registry`](java.rmi.registry.md) | Provides a class and two interfaces for the RMI registry.
| [`java.rmi`](java.rmi.md) | [`java.rmi.server`](java.rmi.server.md) | Provides classes and interfaces for supporting the server side of RMI.
| [`java.base`](java.base.md) | [`java.security`](java.security.md) | Provides the classes and interfaces for the security framework.
| [`java.base`](java.base.md) | [`java.security.cert`](java.security.cert.md) | Provides classes and interfaces for parsing and managing certificates, certificate revocation lists (CRLs), and certification paths.
| [`java.base`](java.base.md) | [`java.security.interfaces`](java.security.interfaces.md) | Provides interfaces for generating RSA (Rivest, Shamir and Adleman AsymmetricCipher algorithm) keys as defined in the RSA Laboratory Technical Note PKCS#1, and DSA (Digital Signature Algorithm) keys as defined in NIST's FIPS-186.
| [`java.base`](java.base.md) | [`java.security.spec`](java.security.spec.md) | Provides classes and interfaces for key specifications and algorithm parameter specifications.
| [`java.sql`](java.sql.md) | [`java.sql`](java.sql.md) | Provides the API for accessing and processing data stored in a data source (usually a relational database) using the Java™ programming language.
| [`java.base`](java.base.md) | [`java.text`](java.text.md) | Provides classes and interfaces for handling text, dates, numbers, and messages in a manner independent of natural languages.
| [`java.base`](java.base.md) | [`java.text.spi`](java.text.spi.md) | Service provider classes for the classes in the java.text package.
| [`java.base`](java.base.md) | [`java.time`](java.time.md) | The main API for dates, times, instants, and durations.
| [`java.base`](java.base.md) | [`java.time.chrono`](java.time.chrono.md) | Generic API for calendar systems other than the default ISO.
| [`java.base`](java.base.md) | [`java.time.format`](java.time.format.md) | Provides classes to print and parse dates and times.
| [`java.base`](java.base.md) | [`java.time.temporal`](java.time.temporal.md) | Access to date and time using fields and units, and date time adjusters.
| [`java.base`](java.base.md) | [`java.time.zone`](java.time.zone.md) | Support for time-zones and their rules.
| [`java.base`](java.base.md) | [`java.util`](java.util.md) | Contains the collections framework, some internationalization support classes, a service loader, properties, random number generation, string parsing and scanning classes, base64 encoding and decoding, a bit array, and several miscellaneous utility classes.
| [`java.base`](java.base.md) | [`java.util.concurrent`](java.util.concurrent.md) | Utility classes commonly useful in concurrent programming.
| [`java.base`](java.base.md) | [`java.util.concurrent.atomic`](java.util.concurrent.atomic.md) | A small toolkit of classes that support lock-free thread-safe programming on single variables.
| [`java.base`](java.base.md) | [`java.util.concurrent.locks`](java.util.concurrent.locks.md) | Interfaces and classes providing a framework for locking and waiting for conditions that is distinct from built-in synchronization and monitors.
| [`java.base`](java.base.md) | [`java.util.function`](java.util.function.md) | *Functional interfaces* provide target types for lambda expressions and method references.
| [`java.base`](java.base.md) | [`java.util.jar`](java.util.jar.md) | Provides classes for reading and writing the JAR (Java ARchive) file format, which is based on the standard ZIP file format with an optional manifest file.
| [`java.util.logging`](java.util.logging.md) | [`java.util.logging`](java.util.logging.md) | Provides the classes and interfaces of the Java™ 2 platform's core logging facilities.
| [`java.prefs`](java.prefs.md) | [`java.util.prefs`](java.util.prefs.md) | This package allows applications to store and retrieve user and system preference and configuration data.
| [`java.base`](java.base.md) | [`java.util.regex`](java.util.regex.md) | Classes for matching character sequences against patterns specified by regular expressions.
| [`java.base`](java.base.md) | [`java.util.spi`](java.util.spi.md) | Service provider classes for the classes in the java.util package.
| [`java.base`](java.base.md) | [`java.util.stream`](java.util.stream.md) | Classes to support functional-style operations on streams of elements, such as map-reduce transformations on collections.
| [`java.base`](java.base.md) | [`java.util.zip`](java.util.zip.md) | Provides classes for reading and writing the standard ZIP and GZIP file formats.

### JavaX

> TODO: What does "JavaX" mean?

> **Is Swing Dead?**
> Apparently Swing is still alive, it's the JApplet class that's deprecated in it.
> The issue is that most of the Swing API is not "thread safe".

| Module | Package | Description |
| :--- | :--- | :--- |
| [`java.desktop`](java.desktop.md) | [`javax.accessibility`](javax.accessibility.md) | Defines a contract between user-interface components and an assistive technology that provides access to those components.
| [`java.compiler`](java.compiler.md) | [`javax.annotation.processing`](javax.annotation.processing.md) | Facilities for declaring annotation processors and for allowing annotation processors to communicate with an annotation processing tool environment.
| [`java.base`](java.base.md) | [`javax.crypto`](javax.crypto.md) | Provides the classes and interfaces for cryptographic operations.
| [`java.base`](java.base.md) | [`javax.crypto.interfaces`](javax.crypto.interfaces.md) | Provides interfaces for Diffie-Hellman keys as defined in RSA Laboratories' PKCS #3.
| [`java.base`](java.base.md) | [`javax.crypto.spec`](javax.crypto.spec.md) | Provides classes and interfaces for key specifications and algorithm parameter specifications.
| [`java.desktop`](java.desktop.md) | [`javax.imageio`](javax.imageio.md) | The main package of the Java Image I/O API.
| [`java.desktop`](java.desktop.md) | [`javax.imageio.event`](javax.imageio.event.md) | A package of the Java Image I/O API dealing with synchronous notification of events during the reading and writing of images.
| [`java.desktop`](java.desktop.md) | [`javax.imageio.metadata`](javax.imageio.metadata.md) | A package of the Java Image I/O API dealing with reading and writing metadata.
| [`java.desktop`](java.desktop.md) | [`javax.imageio.plugins.bmp`](javax.imageio.plugins.bmp.md) | Package containing the public classes used by the built-in BMP plug-in.
| [`java.desktop`](java.desktop.md) | [`javax.imageio.plugins.jpeg`](javax.imageio.plugins.jpeg.md) | Classes supporting the built-in JPEG plug-in.
| [`java.desktop`](java.desktop.md) | [`javax.imageio.plugins.tiff`](javax.imageio.plugins.tiff.md) | Public classes used by the built-in TIFF plug-ins.
| [`java.desktop`](java.desktop.md) | [`javax.imageio.spi`](javax.imageio.spi.md) | A package of the Java Image I/O API containing the plug-in interfaces for readers, writers, transcoders, and streams, and a runtime registry.
| [`java.desktop`](java.desktop.md) | [`javax.imageio.stream`](javax.imageio.stream.md) | A package of the Java Image I/O API dealing with low-level I/O from files and streams.
| [`java.compiler`](java.compiler.md) | [`javax.lang.model`](javax.lang.model.md) | Types and hierarchies of packages comprising a Java language model, a model of the declarations and types of the Java programming language.
| [`java.compiler`](java.compiler.md) | [`javax.lang.model.element`](javax.lang.model.element.md) | Interfaces used to model elements of the Java programming language.
| [`java.compiler`](java.compiler.md) | [`javax.lang.model.type`](javax.lang.model.type.md) | Interfaces used to model Java programming language types.
| [`java.compiler`](java.compiler.md) | [`javax.lang.model.util`](javax.lang.model.util.md) | Utilities to assist in the processing of [program elements](javax.lang.model.element.md) and [types](javax.lang.model.type.md).
| [`java.management`](java.management.md) | [`javax.management`](javax.management.md) | Provides the core classes for the Java Management Extensions.
| [`java.management`](java.management.md) | [`javax.management.loading`](javax.management.loading.md) | Provides the classes which implement advanced dynamic loading.
| [`java.management`](java.management.md) | [`javax.management.modelmbean`](javax.management.modelmbean.md) | Provides the definition of the ModelMBean classes.
| [`java.management`](java.management.md) | [`javax.management.monitor`](javax.management.monitor.md) | Provides the definition of the monitor classes.
| [`java.management`](java.management.md) | [`javax.management.openmbean`](javax.management.openmbean.md) | Provides the open data types and Open MBean descriptor classes.
| [`java.management`](java.management.md) | [`javax.management.relation`](javax.management.relation.md) | Provides the definition of the Relation Service.
| [`java.management`](java.management.md) | [`javax.management.remote`](javax.management.remote.md) | Interfaces for remote access to JMX MBean servers.
| [`java.management.rmi`](java.management.rmi.md) | [`javax.management.remote.rmi`](javax.management.remote.rmi.md) | The RMI connector is a connector for the JMX Remote API that uses RMI to transmit client requests to a remote MBean server.
| [`java.management`](java.management.md) | [`javax.management.timer`](javax.management.timer.md) | Provides the definition of the Timer MBean.
| [`java.naming`](java.naming.md) | [`javax.naming`](javax.naming.md) | Provides the classes and interfaces for accessing naming services.
| [`java.naming`](java.naming.md) | [`javax.naming.directory`](javax.naming.directory.md) | Extends the [`javax.naming`](javax.naming.md) package to provide functionality for accessing directory services.
| [`java.naming`](java.naming.md) | [`javax.naming.event`](javax.naming.event.md) | Provides support for event notification when accessing naming and directory services.
| [`java.naming`](java.naming.md) | [`javax.naming.ldap`](javax.naming.ldap.md) | Provides support for LDAPv3 extended operations and controls.
| [`java.naming`](java.naming.md) | [`javax.naming.ldap.spi`](javax.naming.ldap.spi.md) | N/A 
| [`java.naming`](java.naming.md) | [`javax.naming.spi`](javax.naming.spi.md) | Provides the means for dynamically plugging in support for accessing naming and directory services through the [`javax.naming`](javax.naming.md) and related packages.
| [`java.base`](java.base.md) | [`javax.net`](javax.net.md) | Provides classes for networking applications.
| [`java.base`](java.base.md) | [`javax.net.ssl`](javax.net.ssl.md) | Provides classes for the secure socket package.
| [`java.desktop`](java.desktop.md) | [`javax.print`](javax.print.md) | Provides the principal classes and interfaces for the Java™ Print Service API.
| [`java.desktop`](java.desktop.md) | [`javax.print.attribute`](javax.print.attribute.md) | Provides classes and interfaces that describe the types of Java™ Print Service attributes and how they can be collected into attribute sets.
| [`java.desktop`](java.desktop.md) | [`javax.print.attribute.standard`](javax.print.attribute.standard.md) | Package `javax.print.attribute.standard` contains classes for specific printing attributes.
| [`java.desktop`](java.desktop.md) | [`javax.print.event`](javax.print.event.md) | Package `javax.print.event` contains event classes and listener interfaces.
| [`java.rmi`](java.rmi.md) | [`javax.rmi.ssl`](javax.rmi.ssl.md) | Provides implementations of [`RMIClientSocketFactory`](java.rmi.server.md "interface in java.rmi.server") and [`RMIServerSocketFactory`](java.rmi.server "interface in java.rmi.server") over the Secure Sockets Layer (SSL) or Transport Layer Security (TLS) protocols.
| [`java.scripting`](java.scripting.md) | [`javax.script`](javax.script.md) | The scripting API consists of interfaces and classes that define Java™ Scripting Engines and provides a framework for their use in Java applications.
| [`java.base`](java.base.md) | [`javax.security.auth`](javax.security.auth.md) | This package provides a framework for authentication and authorization.
| [`java.base`](java.base.md) | [`javax.security.auth.callback`](javax.security.auth.callback.md) | This package provides the classes necessary for services to interact with applications in order to retrieve information (authentication data including usernames or passwords, for example) or to display information (error and warning messages, for example).
| [`java.security.jgss`](java.security.jgss.md) | [`javax.security.auth.kerberos`](javax.security.auth.kerberos.md) | This package contains utility classes related to the Kerberos network authentication protocol.
| [`java.base`](java.base.md) | [`javax.security.auth.login`](javax.security.auth.login.md) | This package provides a pluggable authentication framework.
| [`java.base`](java.base.md) | [`javax.security.auth.spi`](javax.security.auth.spi.md) | This package provides the interface to be used for implementing pluggable authentication modules.
| [`java.base`](java.base.md) | [`javax.security.auth.x500`](javax.security.auth.x500.md) | This package contains the classes that should be used to store X500 Principal and X500 Private Credentials in a Subject.
| [`java.base`](java.base.md) | [`javax.security.cert`](javax.security.cert.md) | Provides classes for public key certificates.
| [`java.security.sasl`](java.security.sasl.md) | [`javax.security.sasl`](javax.security.sasl.md) | Contains class and interfaces for supporting SASL.
| [`java.smartcardio`](java.smartcardio.md) | [`javax.smartcardio`](javax.smartcardio.md) | Java™ Smart Card I/O API.
| [`java.desktop`](java.desktop.md) | [`javax.sound.midi`](javax.sound.midi.md) | Provides interfaces and classes for I/O, sequencing, and synthesis of MIDI (Musical Instrument Digital Interface) data.
| [`java.desktop`](java.desktop.md) | [`javax.sound.midi.spi`](javax.sound.midi.spi.md) | Supplies interfaces for service providers to implement when offering new MIDI devices, MIDI file readers and writers, or sound bank readers.
| [`java.desktop`](java.desktop.md) | [`javax.sound.sampled`](javax.sound.sampled.md) | Provides interfaces and classes for capture, processing, and playback of sampled audio data.
| [`java.desktop`](java.desktop.md) | [`javax.sound.sampled.spi`](javax.sound.sampled.spi.md) | Supplies abstract classes for service providers to subclass when offering new audio devices, sound file readers and writers, or audio format converters.
| [`java.sql`](java.sql.md) | [`javax.sql`](javax.sql.md) | Provides the API for server side data source access and processing from the Java™ programming language.
| [`java.sql.rowset`](java.sql.rowset.md) | [`javax.sql.rowset`](javax.sql.rowset.md) | Standard interfaces and base classes for JDBC **`RowSet`** implementations.
| [`java.sql.rowset`](java.sql.rowset.md) | [`javax.sql.rowset.serial`](javax.sql.rowset.serial.md) | Provides utility classes to allow serializable mappings between SQL types and data types in the Java programming language.
| [`java.sql.rowset`](java.sql.rowset.md) | [`javax.sql.rowset.spi`](javax.sql.rowset.spi.md) | The standard classes and interfaces that a third party vendor has to use in its implementation of a synchronization provider.
| [`java.desktop`](java.desktop.md) | `javax.swing` | Provides a set of "lightweight" (all-Java language) components that, to the maximum degree possible, work the same on all platforms.
| [`java.desktop`](java.desktop.md) | `javax.swing.border` | Provides classes and interface for drawing specialized borders around a Swing component.
| [`java.desktop`](java.desktop.md) | `javax.swing.colorchooser` | Contains classes and interfaces used by the `JColorChooser` component.
| [`java.desktop`](java.desktop.md) | `javax.swing.event` | Provides for events fired by Swing components.
| [`java.desktop`](java.desktop.md) | `javax.swing.filechooser` | Contains classes and interfaces used by the `JFileChooser` component.
| [`java.desktop`](java.desktop.md) | `javax.swing.plaf` | Provides one interface and many abstract classes that Swing uses to provide its pluggable look-and-feel capabilities.
| [`java.desktop`](java.desktop.md) | `javax.swing.plaf.basic` | Provides user interface objects built according to the Basic look and feel.
| [`java.desktop`](java.desktop.md) | `javax.swing.plaf.metal` | Provides user interface objects built according to the Java look and feel (once codenamed Metal), which is the default look and feel.
| [`java.desktop`](java.desktop.md) | `javax.swing.plaf.multi` | Provides user interface objects that combine two or more look and feels.
| [`java.desktop`](java.desktop.md) | `javax.swing.plaf.nimbus` | Provides user interface objects built according to the cross-platform Nimbus look and feel.
| [`java.desktop`](java.desktop.md) | `javax.swing.plaf.synth` | Synth is a skinnable look and feel in which all painting is delegated.
| [`java.desktop`](java.desktop.md) | `javax.swing.table` | Provides classes and interfaces for dealing with `javax.swing.JTable`.
| [`java.desktop`](java.desktop.md) | `javax.swing.text` | Provides classes and interfaces that deal with editable and noneditable text components.
| [`java.desktop`](java.desktop.md) | `javax.swing.text.html` | Provides the class `HTMLEditorKit` and supporting classes for creating HTML text editors.
| [`java.desktop`](java.desktop.md) | `javax.swing.text.html.parser` | Provides the default HTML parser, along with support classes.
| [`java.desktop`](java.desktop.md) | `javax.swing.text.rtf` | Provides a class (`RTFEditorKit`) for creating Rich-Text-Format text editors.
| [`java.desktop`](java.desktop.md) | `javax.swing.tree` | Provides classes and interfaces for dealing with `javax.swing.JTree`.
| [`java.desktop`](java.desktop.md) | `javax.swing.undo` | Allows developers to provide support for undo/redo in applications such as text editors.
| [`java.compiler`](java.compiler.md) | [`javax.tools`](javax.tools.md) | Provides interfaces for tools which can be invoked from a program, for example, compilers.
| [`java.transaction.xa`](java.transaction.xa.md) | [`javax.transaction.xa`](javax.transaction.xa.md) | Provides the API that defines the contract between the transaction manager and the resource manager, which allows the transaction manager to enlist and delist resource objects (supplied by the resource manager driver) in JTA transactions.
| [`java.xml`](java.xml.md) | [`javax.xml`](javax.xml.md) | Defines constants for XML processing.
| [`java.xml`](java.xml.md) | [`javax.xml.catalog`](javax.xml.catalog.md) | Provides the classes for implementing [XML Catalogs OASIS Standard V1.1, 7 October 2005](https://www.oasis-open.org/committees/download.php/14809/xml-catalogs.html).
| [`java.xml.crypto`](java.xml.crypto.md) | [`javax.xml.crypto`](javax.xml.crypto.md) | Common classes for XML cryptography.
| [`java.xml.crypto`](java.xml.crypto.md) | [`javax.xml.crypto.dom`](javax.xml.crypto.dom.md) | DOM-specific classes for the [`javax.xml.crypto`](javax.xml.crypto.md) package.
| [`java.xml.crypto`](java.xml.crypto.md) | [`javax.xml.crypto.dsig`](javax.xml.crypto.dsig.md) | Classes for generating and validating XML digital signatures.
| [`java.xml.crypto`](java.xml.crypto.md) | [`javax.xml.crypto.dsig.dom`](javax.xml.crypto.dsig.dom.md) | DOM-specific classes for the [`javax.xml.crypto.dsig`](javax.xml.crypto.dsig.md) package.
| [`java.xml.crypto`](java.xml.crypto.md) | [`javax.xml.crypto.dsig.keyinfo`](javax.xml.crypto.dsig.keyinfo.md) | Classes for parsing and processing [`KeyInfo`](javax.xml.crypto.dsig.keyinfo.md "interface in javax.xml.crypto.dsig.keyinfo") elements and structures.
| [`java.xml.crypto`](java.xml.crypto.md) | [`javax.xml.crypto.dsig.spec`](javax.xml.crypto.dsig.spec.md) | Parameter classes for XML digital signatures.
| [`java.xml`](java.xml.md) | [`javax.xml.datatype`](javax.xml.datatype.md) | Defines XML/Java Type Mappings.
| [`java.xml`](java.xml.md) | [`javax.xml.namespace`](javax.xml.namespace.md) | Defines XML Namespace processing.
| [`java.xml`](java.xml.md) | [`javax.xml.parsers`](javax.xml.parsers.md) | Provides the classes for processing XML documents with a SAX (Simple API for XML) parser or a DOM (Document Object Model) Document builder.
| [`java.xml`](java.xml.md) | [`javax.xml.stream`](javax.xml.stream.md) | Defines interfaces and classes for the Streaming API for XML (StAX).
| [`java.xml`](java.xml.md) | [`javax.xml.stream.events`](javax.xml.stream.events.md) | Defines event interfaces for the Streaming API for XML (StAX).
| [`java.xml`](java.xml.md) | [`javax.xml.stream.util`](javax.xml.stream.util.md) | Provides utility classes for the Streaming API for XML (StAX).
| [`java.xml`](java.xml.md) | [`javax.xml.transform`](javax.xml.transform.md) | Defines the generic APIs for processing transformation instructions, and performing a transformation from source to result.
| [`java.xml`](java.xml.md) | [`javax.xml.transform.dom`](javax.xml.transform.dom.md) | Provides DOM specific transformation classes.
| [`java.xml`](java.xml.md) | [`javax.xml.transform.sax`](javax.xml.transform.sax.md) | Provides SAX specific transformation classes.
| [`java.xml`](java.xml.md) | [`javax.xml.transform.stax`](javax.xml.transform.stax.md) | Provides StAX specific transformation classes.
| [`java.xml`](java.xml.md) | [`javax.xml.transform.stream`](javax.xml.transform.stream.md) | Provides stream and URI specific transformation classes.
| [`java.xml`](java.xml.md) | [`javax.xml.validation`](javax.xml.validation.md) | Provides an API for validation of XML documents.
| [`java.xml`](java.xml.md) | [`javax.xml.xpath`](javax.xml.xpath.md) | Provides an *object-model neutral* API for the evaluation of XPath expressions and access to the evaluation environment.

### JDK

| Modules | Package | Description |
| :--- | :--- | :--- |
| [`jdk.dynalink`](jdk.dynalink.md) | [`jdk.dynalink`](jdk.dynalink.md) | Contains interfaces and classes that are used to link an `invokedynamic` call site.
| [`jdk.dynalink`](jdk.dynalink.md) | [`jdk.dynalink.beans`](jdk.dynalink.beans.md) | Contains the linker for ordinary Java objects.
| [`jdk.dynalink`](jdk.dynalink.md) | [`jdk.dynalink.linker`](jdk.dynalink.linker.md) | Contains interfaces and classes needed by language runtimes to implement their own language-specific object models and type conversions.
| [`jdk.dynalink`](jdk.dynalink.md) | [`jdk.dynalink.linker.support`](jdk.dynalink.linker.support.md) | Contains classes that make it more convenient for language runtimes to implement their own language-specific object models and type conversions by providing basic implementations of some classes as well as various utilities.
| [`jdk.dynalink`](jdk.dynalink.md) | [`jdk.dynalink.support`](jdk.dynalink.support.md) | Contains classes that make using Dynalink more convenient by providing basic implementations of some classes as well as various utilities.
| [`jdk.incubator.foreign`](jdk.incubator.foreign.md) | [`jdk.incubator.foreign`](jdk.incubator.foreign.md) | Classes to support low-level, safe and efficient memory access.
| [`jdk.javadoc`](jdk.javadoc.md)  | [`jdk.javadoc.doclet`](jdk.javadoc.doclet.md) | The Doclet API provides an environment which, in conjunction with the Language Model API and Compiler Tree API, allows clients to inspect the source-level structures of programs and libraries, including API comments embedded in the source.
| [`jdk.jfr`](jdk.jfr.md) | [`jdk.jfr`](jdk.jfr.md) | This package provides classes to create events and control Flight Recorder.
| [`jdk.jfr`](jdk.jfr.md) | [`jdk.jfr.consumer`](jdk.jfr.consumer.md) | This package contains classes for consuming Flight Recorder data.
| [`jdk.jshell`](jdk.jshell.md) | [`jdk.jshell`](jdk.jshell.md) | Provides interfaces for creating tools, such as a Read-Eval-Print Loop (REPL), which interactively evaluate "snippets" of Java programming language code.
| [`jdk.jshell`](jdk.jshell.md) | [`jdk.jshell.execution`](jdk.jshell.execution.md) | Provides implementation support for building JShell execution engines.
| [`jdk.jshell`](jdk.jshell.md) | [`jdk.jshell.spi`](jdk.jshell.spi.md) | Defines the Service Provider Interface for pluggable JShell execution engines.
| [`jdk.jshell`](jdk.jshell.md) | [`jdk.jshell.tool`](jdk.jshell.tool.md) | Provides a mechanism to launch an instance of a Java™ shell tool.
| [`jdk.management.jfr`](jdk.management.jfr.md) | [`jdk.management.jfr`](jdk.management.jfr.md) | This package contains classes to control and monitor Flight Recorder over Java Management Extensions (JMX).
| ~~`jdk.scripting.nashorn`~~ | ~~`jdk.nashorn.api.scripting`~~ | ~~This package provides the [`javax.script`](javax.script.md) integration, which is the preferred way to use Nashorn.~~ **Deprecated**
| ~~`jdk.scripting.nashorn`~~ | ~~`jdk.nashorn.api.tree`~~ | ~~Nashorn parser API provides interfaces to represent ECMAScript source code as abstract syntax trees (AST) and Parser to parse ECMAScript source scripts.~~ **Deprecated**
| [`jdk.net`](jdk.net.md) | [`jdk.net`](jdk.net.md) | Platform specific socket options for the [`java.net`](java.net.md) and [`java.nio.channels`](java.nio.channels.md) socket classes.
| [`jdk.net`](jdk.net.md) | [`jdk.nio`](jdk.nio.md) | Defines JDK-specific [channel](java.nio.channels.md "interface in java.nio.channels") APIs.
| [`jdk.jartool`](jdk.jartool.md) | [`jdk.security.jarsigner`](jdk.security.jarsigner.md) | This package defines APIs for signing jar files.

### Internet Stuff

> "'Netscape.' That's a name I haven't heard in many years." --Old Ben
> Yes, that module is STILL relevant!

| Modules | Package | Description |
| :--- | :--- | :--- |
| [`jdk.jsobject`](jdk.jsobject.md) | [`netscape.javascript`](netscape.javascript.md) | Provides Java code the ability to access the JavaScript engine and the HTML DOM in the web browser. (This is probably Old AF!)
| [`java.security.jgss`](java.security.jgss.md) | [`org.ietf.jgss`](org.ietf.jgss.md) | This package presents a framework that allows application developers to make use of security services like authentication, data integrity and data confidentiality from a variety of underlying security mechanisms like Kerberos, using a unified API.
| [`java.xml`](java.xml.md) | [`org.w3c.dom`](org.w3c.dom.md) | Provides the interfaces for the Document Object Model (DOM).
| [`java.xml`](java.xml.md) | [`org.w3c.dom.bootstrap`](org.w3c.dom.bootstrap.md) | Provides a factory for obtaining instances of `DOMImplementation`.
| [`jdk.xml.dom`](jdk.xml.dom.md) | [`org.w3c.dom.css`](org.w3c.dom.css.md) | Provides interfaces for DOM Level 2 Style Specification.
| [`java.xml`](java.xml.md) | [`org.w3c.dom.events`](org.w3c.dom.events.md) | Provides interfaces for DOM Level 2 Events.
| [`jdk.xml.dom`](jdk.xml.dom.md) | [`org.w3c.dom.html`](org.w3c.dom.html.md) | Provides interfaces for DOM Level 2 HTML Specification.
| [`java.xml`](java.xml.md) | [`org.w3c.dom.ls`](org.w3c.dom.ls.md) | Provides interfaces for DOM Level 3 Load and Save.
| [`java.xml`](java.xml.md) | [`org.w3c.dom.ranges`](org.w3c.dom.ranges.md) | Provides interfaces for DOM Level 2 Range.
| [`jdk.xml.dom`](jdk.xml.dom.md) | [`org.w3c.dom.stylesheets`](org.w3c.dom.stylesheets.md) | Provides interfaces for DOM Level 2 Style Specification.
| [`java.xml`](java.xml.md) | [`org.w3c.dom.traversal`](org.w3c.dom.traversal.md) | Provides interfaces for DOM Level 2 Traversal.
| [`java.xml`](java.xml.md) | [`org.w3c.dom.views`](org.w3c.dom.views.md) | Provides interfaces for DOM Level 2 Views.
| [`jdk.xml.dom`](jdk.xml.dom.md) | [`org.w3c.dom.xpath`](org.w3c.dom.xpath.md) | Provides interfaces for DOM Level 3 XPath Specification.
| [`java.xml`](java.xml.md) | [`org.xml.sax`](org.xml.sax.md) | Provides the interfaces for the Simple API for XML (SAX).
| [`java.xml`](java.xml.md) | [`org.xml.sax.ext`](org.xml.sax.ext.md) | Provides interfaces to SAX2 facilities that conformant SAX drivers won't necessarily support.
| [`java.xml`](java.xml.md) | [`org.xml.sax.helpers`](org.xml.sax.helpers.md) | Provides helper classes, including support for bootstrapping SAX-based applications.

## See Also

* [All Classes](all_classes.md)

## Sources

* Oracle. [All Packages (Java SE 14 & JDK 14)](https://docs.oracle.com/en/java/javase/14/docs/api/allpackages-index.html). 18 May 2020.
* Oracle. [Depricated List (Java SE 14 & JDK 14)](https://docs.oracle.com/en/java/javase/14/docs/api/deprecated-list.html). 18 May 2020.