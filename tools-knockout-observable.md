---
date: 2020-10-30T11:37
tags:
  - tools/knockout/
---

# Knockout Observables

## Model

A Knockout *model* includes
* data
* operations

that represent the business domain of the application.

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

### tools-knockout-observable