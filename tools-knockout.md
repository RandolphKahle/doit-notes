---
date: 2020-10-30T11:02
---

# KnockOut

Javascript library for web UI development - data binding and form management.

Knockout uses an MVVM approach. A:
* **Model** – contains the business domain including data and functions
* **View** - user interface
* **View-Model** - In-flight data that backs the UI. Any changes made by the user are stored here. Includes functions to support UI operations such as dropping or adding elements in a set or array.

```
UI <--> View-Model <--> Model <--(Ajax)--> Server
```

The core concepts are:
* Observables
* Bindings
* Templating


## Model

A Knockout *model* comprises the business domain:
* data
* operations

The communication with the server involves retrieving and sending this model via Ajax calls.

## View Model

A *pure-code* representation of data and operations within and supporting a user interface (UI).

For example, for a list editor, the view-model is an object holding a list of items and exposes methods to add and remove items.

This is the temporary, in-memory, interm storage of information the user is working on.

## View

The visible interactive user interface that represents the state of the *view-model*. The view sends commands to the *view-model* (e.g. when a user clicks a button) and updates whenever the state of the *view-model* changes.

## Binding

A Binding links a *view* with a *view-model*.

The *view* contains declarative bindings that link it to the *view-model*.


### tools-knockout
