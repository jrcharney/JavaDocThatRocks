# Package `java.lang`

## Description

**`java.lang`** provides classes that are fundamental to the design of the Java programming language. The most important classes are [**`Object`**](java.lang.Object.md), which is the root of the class hierarchy, and **`Class`**, instances of which represent classes at run time.

Frequently, it is necessary to represent a value of primitive type as if it were an object. The wrapper classes **`Boolean`**, **`Character`**, **`Integer`**, **`Long`**, **`Float`**, and **`Double`** serve this purpose. An object of type `Double`, for example, contains a field whose type is `double`, representing that value in such a way that a reference to it can be stored in a variable of reference type. These classes also provide a number of methods for converting among primitive values, as well as supporting such standard methods as `equals` and `hashCode`. The **`Void`** class is a non-instantiable class that holds a reference to a `Class` object representing the type `void`.

The class **`Math`** provides commonly used mathematical functions such as sine, cosine, and square root. The classes **`String`**, **`StringBuffer`**, and **`StringBuilder`** similarly provide commonly used operations on character strings.

Classes **`ClassLoader`**, **`Process`**, **`ProcessBuilder`**, **`Runtime`**, **`SecurityManager`**, and **`System`** provide "system operations" that manage the dynamic loading of classes, creation of external processes, host environment inquiries such as the time of day, and enforcement of security policies.

Class **`Throwable`** encompasses objects that may be thrown by the `throw` statement. Subclasses of `Throwable` represent errors and exceptions.

### Character Encodings

The specification of the `java.nio.charset.Charset` class describes the naming conventions for character encodings as well as the set of standard encodings that must be supported by every implementation of the Java platform.

## Interfaces

| Interface | Description |
| :--- | :--- |
| [`Appendable`](java.lang.Appendable.md) | An object to which char sequences and values can be appended.
| [`AutoCloseable`](java.lang.AutoCloseable.md) | An object that may hold resources (such as file or socket handles) until it is closed.
| [`CharSequence`](java.lang.CharSequence.md) | A `CharSequence` is a readable sequence of `char` values.
| [`Cloneable`](java.lang.Cloenable.md) | A class implements the `Cloneable` interface to indicate to the `Object.clone()` method that it is legal for that method to make a field-for-field copy of instances of that class.
| [`Comparable`](java.lang.Comparable.md)`<T>` | This interface imposes a total ordering on the objects of each class that implements it.
| [`Iterable`](java.lang.Iterable.md)`<T>` | Implementing this interface allows an object to be the target of the enhanced for statement (sometimes called the "for-each loop" statement).
| [`ProcessHandle`](java.lang.ProcessHandle.md) | `ProcessHandle` identifies and provides control of native processes.
| `ProcessHandle.Info` | Information snapshot about the process.
| [`Readable`](java.lang.Readable.md) | A `Readable` is a source of characters.
| [`Runnable`](java.lang.Runnable.md) | The `Runnable` interface should be implemented by any class whose instances are intended to be executed by a thread.
| `StackWalker.StackFrame` | A `StackFrame` object represents a method invocation returned by `StackWalker`.
| [`System.Logger`](java.lang.System.Logger.md) | `System.Logger` instances log messages that will be routed to the underlying logging framework the `LoggerFinder` uses.
| [`Thread.UncaughtExceptionHandler`](java.lang.Thread.UncaughtExceptionHandler.md) | Interface for handlers invoked when a `Thread` abruptly terminates due to an uncaught exception.

## Classes

## Enums

## Exceptions

## Annotations