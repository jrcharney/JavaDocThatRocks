# Modules

## `java.*` (Java SE)

**The Java Platform, Standard Edition** (Java SE) APIs define the core Java platform for general-purpose computing. These APIs are in modules whose names start with `java`.

| Module | Description |
| :--- | :--- |
| [`java.base`](java.base.md) | Defines the foundational APIs of the Java SE Platform.
| [`java.compiler`](java.compiler.md) | Defines the Language Model, Annotation Processing, and Java Compiler APIs.
| [`java.datatransfer`](java.datatransfer.md) | Defines the API for transferring data between and within applications.
| [`java.desktop`](java.desktop.md)| Defines the AWT and Swing user interface toolkits, plus APIs for accessibility, audio, imaging, printing, and JavaBeans.
| [`java.instrument`](java.instrument.md) | Defines services that allow agents to instrument programs running on the JVM.
| [`java.logging`](java.logging.md) | Defines the Java Logging API.
| [`java.management`](java.management.md) | Defines the Java Management Extensions (JMX) API.
| [`java.management.rmi`](java.management.rmi.md) | Defines the RMI connector for the Java Management Extensions (JMX) Remote API.
| [`java.naming`](java.naming.md) | Defines the Java Naming and Directory Interface (JNDI) API.
| [`java.net.http`](java.net.http.md) | Defines the HTTP Client and WebSocket APIs.
| [`java.prefs`](java.prefs.md) | Defines the Preferences API.
| [`java.rmi`](java.rmi.md) | Defines the Remote Method Invocation (RMI) API.
| [`java.scripting`](java.scripting.md) | Defines the Scripting API.
| [`java.se`](java.se.md) | Defines the API of the Java SE Platform.
| [`java.security.jgss`](java.security.jgss.md) | Defines the Java binding of the IETF Generic Security Services API (GSS-API).
| [`java.security.sasl`](java.security.sasl.md) | Defines Java support for the IETF Simple Authentication and Security Layer (SASL).
| [`java.sql`](java.sql.md) | Defines the JDBC API.
| [`java.sql.rowset`](java.sql.rowset.md) | Defines the JDBC RowSet API.
| [`java.transaction.xa`](java.transaction.xa.md) | Defines an API for supporting distributed transactions in JDBC.
| [`java.xml`](java.xml.md) | Defines the Java API for XML Processing (JAXP), the Streaming API for XML (StAX), the Simple API for XML (SAX), and the W3C Document Object Model (DOM) API.
| [`java.xml.crypto`](java.xml.crypto.md) | Defines the API for XML cryptography.

## `jdk.*` (JDK)

**The Java Development Kit** (JDK) APIs are specific to the JDK and will not necessarily be available in all implementations of the Java SE Platform. These APIs are in modules whose names start with `jdk`.

| Module | Description |
| :--- | :--- |
| [`jdk.accessibility`](jdk.accessibility.md) | Defines JDK utility classes used by implementors of Assistive Technologies.
| [`jdk.attach`](jdk.attach.md) | Defines the attach API.
| [`jdk.charsets`](jdk.charsets.md) | Provides `charsets` that are not in `java.base` (mostly double byte and IBM charsets).
| [`jdk.compiler`](jdk.compiler.md) | Defines the implementation of the system Java compiler and its command line equivalent, `javac`.
| [`jdk.crypto.cryptoki`](jdk.crypto.cryptoki.md) | Provides the implementation of the SunPKCS11 security provider.
| [`jdk.crypto.ec`](jdk.crypto.ec.md) | Provides the implementation of the SunEC security provider.
| [`jdk.dynalink`](jdk.dynalink.md) | Defines the API for dynamic linking of high-level operations on objects.
| [`jdk.editpad`](jdk.editpad.md) | Provides the implementation of the edit pad service used by `jdk.jshell`.
| [`jdk.hotspot.agent`](jdk.hotspot.agent.md) | Defines the implementation of the HotSpot Serviceability Agent.
| [`jdk.httpserver`](jdk.httpserver.md) | Defines the JDK-specific HTTP server API.
| [`jdk.incubator.foreign`](jdk.incubator.foreign.md) | Defines the experimental foreign memory access API.
| [`jdk.incubator.jpackage`](jdk.incubator.jpackage.md) | Defines the Java Packaging tool, `jpackage`.
| ([`jdk.jartool`](jdk.jartool.md) | Defines tools for manipulating Java Archive (JAR) files, including the `jar` ~~and `jarsigner`~~ tools.
| [`jdk.javadoc`](jdk.javadoc.md) | Defines the implementation of the system documentation tool and its command line equivalent, javadoc.
| [`jdk.jcmd`](jdk.jcmd.md) | Defines tools for diagnostics and troubleshooting a JVM such as the `jcmd`, `jps`, `jstat` tools.
| [`jdk.jconsole`](jdk.jconsole.md) |	Defines the JMX graphical tool, `jconsole`, for monitoring and managing a running application.
| [`jdk.jdeps`](jdk.jdeps.md) | Defines tools for analysing dependencies in Java libraries and programs, including the `jdeps`, `javap`, and `jdeprscan` tools.
| [`jdk.jdi`](jdk.jdi.md) | Defines the Java Debug Interface.
| [`jdk.jdwp.agent`](jdk.jdwp.agent.md) | Provides the implementation of the Java Debug Wire Protocol (JDWP) agent.
| [`jdk.jfr`](jdk.jfr.md) | Defines the API for JDK Flight Recorder.
| [`jdk.jlink`](jdk.jlink.md) | Defines the `jlink` tool for creating run-time images, the `jmod` tool for creating and manipulating JMOD files, and the `jimage` tool for inspecting the JDK implementation-specific container file for classes and resources.
| [`jdk.jshell`](jdk.jshell.md) | Provides the `jshell` tool for evaluating snippets of Java code, and defines a JDK-specific API for modeling and executing snippets.
| [`jdk.jsobject`](jdk.jsobject.md) | Defines the API for the JavaScript Object.
| [`jdk.jstatd`](jdk.jstatd.md) | Defines the `jstatd` tool for starting a daemon for the `jstat` tool to monitor JVM statistics remotely.
| [`jdk.localedata`](jdk.localedata.md) | Provides the locale data for locales other than US locale.
| [`jdk.management`](jdk.management.md) | Defines JDK-specific management interfaces for the JVM.
| [`jdk.management.agent`](jdk.management.agent.md) | Defines the JMX management agent.
| [`jdk.management.jfr`](jdk.management.jfr.md) | Defines the Management Interface for JDK Flight Recorder.
| [`jdk.naming.dns`](jdk.naming.dns.md) | Provides the implementation of the DNS Java Naming provider.
| [`jdk.naming.rmi`](jdk.naming.rmi.md) | Provides the implementation of the RMI Java Naming provider.
| [`jdk.net`](jdk.net.md) | Defines the JDK-specific Networking API.
| [`jdk.rmic`](jdk.rmic.md) | Defines the `rmic` compiler for generating stubs and skeletons using the Java Remote Method Protocol (JRMP) for remote objects.
| ~~`jdk.scripting.nashorn`~~ | ~~Provides the implementation of Nashorn script engine and the runtime environment for programs written in ECMAScript 5.1.~~ **Deprecated**
| [`jdk.sctp`](jdk.sctp.md) | Defines the JDK-specific API for SCTP.
| [`jdk.security.auth`](jdk.security.auth.md) | Provides implementations of the `javax.security.auth.*` interfaces and various authentication modules.
| [`jdk.security.jgss`](jdk.security.jgss.md) | Defines JDK extensions to the GSS-API and an implementation of the SASL GSSAPI mechanism.
| [`jdk.xml.dom`](jdk.xml.dom.md) | Defines the subset of the W3C Document Object Model (DOM) API that is not part of the Java SE API.
| [`jdk.zipfs`](jdk.zipfs.md) | Provides the implementation of the Zip file system provider.

## Other Modules

| Module | Description |
| :--- | :--- |
| [`java.smartcardio`](java.smartcardio.md) | Defines the Java Smart Card I/O API |
