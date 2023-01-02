.. _printing-hello-world:

Printing Hello World
====================

Learning how to print `Hello World!` is the most conventional or de facto
technique to commence learning a new programming language, whether it be Java or
any other language in general. Every language has its own syntax, which
inevitably introduces or better yet, refreshes a few concepts. Java is no
different. Despite being wide and somewhat beginner-friendly language, Java
nevertheless demands some basic programming paradigm knowledge from the user. 

Let's learn how to print a straightforward `Hello World!` in Java and the
concepts that underlie its verbose syntax.

.. code-block:: java

    public class MyHelloWorldClass {
        public static void main(String[] args) {
            System.out.println("Hello Hello World!");
        }
    }

Java's Philosophy
-----------------

As Java is an `Object Oriented Language`_, every entity which is created in it
should be something called as `Class-Based`_ or should be `Class-Oriented`.
Thus, everything you do OR create in Java, i.e attributes or methods should be
encapsulated in a class. That's why even when you wanna print something, it has
to be put through a class and it's respective method. There are a couple of
things the user needs to be aware of prior creating a new classes.

#. It is said that every class in Java should be written in it's own file (.java)
   file. It's considered as one of it's best practices. The file name should be
   maintained in PascalCase OR `CamelCase`_ and so is the class name.
#. The file name and the class name should be the same.

.. note::

    There are other notable concepts like packages, etc. but for now let's just
    focus on writing a simple java file. To read about packages, see THIS.

Breakdown of the Hello World! syntax
------------------------------------

So now that you know about the class definition and it's significance in Java,
let's focus on the following lines of code.

.. code-block:: java

    public static void main(String[] args) {
        System.out.println("Hello Hello World!");
    }

public
~~~~~~

Here, the keyword `public` is something called as an `Access Modifier`_. In
short, an `Access Modifier` is an entity that is used to set the access level of
for the classes, attributes and methods. Basically, it provides access level
control -- What, Who and How something can be accessed.

There are two types of **Modifiers**: Access and Non-Access Modifiers

Access Modifiers which controls the access level and Non-Access Modifiers which do
not control the access level but provides other functionalities. We'll focus
more on the Access Modifiers here.

A ``public`` access modifier can be declared by a class, method, constructor,
interface, etc. and can be accessed by any other class. Therefore, anything
which is declared inside a public class can be accessed from any class in Java.

.. note::

    If the public class is in a different package, then public class needs
    to be imported.

There are different types of access modifiers: Public, Private, Protected and
Default. Those are not that important while understanding the concept of
learning `Hello World!` though.

When methods, variables, classes, etc are declared as public, then we can access
them from anywhere. The public access modifiers has no scope restriction.

Consider this example:

.. code-block:: java

    // The below code is defined in file called Dexter.java
    public class Dexter {
        public int someVariable;
    }

    // The below code is defined in file called Main.java
    public class Main {
        public static void main(String[] args) {
            Dexter dexter = new Dexter();
            dexter.someVariable = 42;
        }
    }

.. Mention all the external references here

.. _Object Oriented Language: https://en.wikipedia.org/wiki/Object-oriented_programming
.. _Class-Based: https://en.wikipedia.org/wiki/Class-based_programming
.. _CamelCase: https://en.wikipedia.org/wiki/Camel_case
.. _Access Modifier: https://www.javatpoint.com/access-modifiers
