# Introduction

A [Giter8][g8] template for generating a document based on
[Tufte-Latex](https://tufte-latex.github.io/tufte-latex/), a Tufte-inspired LaTeX class for producing books.

# Prerequisites

You need [Giter8][g8] installed.

# Creating a Project

To create a new working project invoke giter8 using the giter8 template:
```console
foo@bar:~$ g8 jerrykuch/tufte-latex-book.g8
```
Answer 

# Project Structure



```java
ST.render()
```

For example, the following template has two chunks, a literal and a reference to attribute `name`:

```
Hello, <name>
```

Using templates in code is very easy. Here is the requisite example that prints `Hello, World`:

```java
import org.stringtemplate.v4.*;
...
ST hello = new ST("Hello, <name>");
hello.add("name", "World");
System.out.println(hello.render());
```

|MVC Pattern|
|-----------|
|In the parlance of the model-view-controller (MVC) pattern, templates represent the view and the code fragment represents both model (the name string) and controller (that pulls from the model and injects attributes into the view).|

StringTemplate is not a "system" or "engine" or "server". It is designed to be embedded inside other applications and is distributed as a small library with no external dependencies except ANTLR (used for parsing the StringTemplate template language).

## Groups of templates

The primary classes of interest are `ST`, `STGroupDir`, and `STGroupFile`. You can directly create a template in code, you can load templates from a directory, and you can load a file containing a collection of templates (a template group file). Group files behave like zips or jars of template directories.

For example, let's assume we have two templates in files `decl.st` and `init.st` in directory `/tmp`:

```
// file /tmp/decl.st
decl(type, name, value) ::= "<type> <name><init(value)>;"
```
