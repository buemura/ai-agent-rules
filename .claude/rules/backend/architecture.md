# Rules for Architecture

## This file describes the architectural rules for the project.

The project should follow a modular monolithic architecture, where the codebase is organized into modules that encapsulate specific functionality. Each module should have a clear responsibility and should interact with other modules through well-defined interfaces.
The project should also follow the principles of separation of concerns, where different aspects of the application are separated into different layers. For example, the presentation layer should be responsible for handling user interactions and displaying data, while the business logic layer should be responsible for processing data and implementing the core functionality of the application.
The project should also follow the principles of SOLID design, which include:

- Single Responsibility Principle: Each module should have only one reason to change.
- Open/Closed Principle: Modules should be open for extension but closed for modification.
- Liskov Substitution Principle: Subtypes should be substitutable for their base types.
- Interface Segregation Principle: Clients should not be forced to depend on interfaces they do not use.
- Dependency Inversion Principle: High-level modules should not depend on low-level modules. Both should depend on abstractions.

### File structure

- All source code files should be placed in the `src` directory.
- The configuration files should be placed in the `src/configs` directory.
- The shared utilities like (helper functions, database client, queue client, etc.) should be placed in the `src/shared` directory.
- The API should be separated into different modules based on functionality, and each module should have its own directory under `src/modules`. A module should contain all the necessary files for its functionality, including models, controllers, services, and routes. Each module should have its own `index.ts` file that exports the main functionality of the module.
- The interaction between modules should be done through well-defined interfaces/clients, and the modules should not have direct dependencies on each other. Instead, they should communicate through a shared interface or a message bus.
