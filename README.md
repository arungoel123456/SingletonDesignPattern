# SingletonDesignPattern

## Overview
This repository contains a simple implementation of an application logger to demonstrate the **Singleton Design Pattern**. The Singleton pattern ensures that a class has only one instance and provides a global point of access to that instance. In this project, the logger is used as an example of how the Singleton pattern can be applied to restrict instantiation of a logging class to just one object.

## Features
- Ensures that only one instance of the logger is created.
- Provides a simple API to log messages (e.g., `info`, `warn`, `error`).
- Thread-safe, making sure the Singleton instance is accessible in multi-threaded applications.

## Why Singleton?
The Singleton pattern is useful when:
- Exactly one instance of a class is needed, like in the case of a logger.
- You want to control access to shared resources.
- You need global access to the instance across your application without recreating it.

## How it Works
The application logger restricts instantiation of the logger class by:
1. Making the constructor private (or inaccessible).
2. Providing a static method to get the instance of the class (`get_instance`).
3. Ensuring that only one instance is created, even when accessed by multiple clients.
