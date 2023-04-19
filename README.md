# Flutter Clean Geolocation

Pair Programming of a Production Ready Geolocation App using Flutter

This repository is following [**Clean Geolocation Tutorial with Flutter**](https://www.youtube.com/playlist?list=PLwYCg1QCF6vDZEo7NnvQ2Jx8ITsBiUguU) playlist.

## Introduction

We're building a map app for IOS and Android devices.

After the user gives required permissions it will show the user's location on th map with a maker.

**What makes this project different? ** **What will we focus on?**

- Building a snappy app with scalable architecture
- Displaying aproper way of handling state management
- Showing how to orchestrate packages
- Handling edge cases
- How to separate business logic from ui
- Making user friendly UX

## Architecture

[Domain-Driven Design Principles - Reso Coder](https://resocoder.com/2020/03/09/flutter-firebase-ddd-course-1-domain-driven-design-principles/)

![img](https://resocoder.com/wp-content/uploads/2020/03/DDD-Flutter-Diagram-v3.svg)

## Clean Way to Handle State Management

### Why [flutter_bloc](https://pub.dev/packages/flutter_bloc)?

- Separate business logic from UI easily
- Testable
- Highly maintained

### Why [Cubit](https://bloclibrary.dev/#/coreconcepts?id=cubit)?

- Subset of [Bloc](https://bloclibrary.dev/#/coreconcepts?id=bloc)
- Less boilerplate
- Easy to understand

![Cubit Architecture](https://bloclibrary.dev/assets/cubit_architecture_full.png)

### Why [freezed](https://pub.dev/packages/freezed) in states?

- Immutable by defalut
- Less error prone
- Reduced  boilerplate
- Implements value equality
- Supports union types for mutually exclusive states

Also usefly for:

- Serialization/deserialization
- Model classes
- Alternative for enums

### Dependency Injection

Why [injectable](https://pub.dev/packages/injectable)?

- Generates [git_it](https://pub.dev/packages/injectable) code
- Automates registration of dependencies
- Decreases coupling between classes and their dependencies

