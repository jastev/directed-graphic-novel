# Goal

The goal of the project is twofold: to showcase the breadth of Azure's support
for various languages, datastores, and PaaS architectures; and to provide
example code for each that are directly comparable to each other, for learning
purposes.

Ideally, developers who are familiar with one combination of these should be
able to find an apples-to-apples implementation in the target architecture,
and be able to use the comparison as a guide to help them with their own
projects.

# Approach

We define a specification and architecture-agnostic design for a simple web
app.  The [spec](spec.md) is detailed enough to lead to highly comparable
implementations, while providing enough abstraction to allow for idiomatic
use of different languages, platforms, and data stores.

Each implementation provides the same REST API.  A single web client is defined
that can be used against any of the API implementations.

# The Directed Graphic Novel

The theme for the spec is a story where the reader must make choices at the
end of each page - the plot is thus different depending upon the choices made.
These thus form a directed graph, where the pages are vertices in the graph and
the choices are edges (a given page may not have the option to reverse the
previous choice, hence the following page must have a choice to return if this
is to be available to the reader, and thus the graph is directed).