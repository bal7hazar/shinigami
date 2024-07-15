# Shinigami

Shinigami is designed for creating fully onchain games within Autonomous Worlds on Starknet. Feedback and contributions are welcome!

Shinigami follows a structured approach to enable efficient development and maintenance of onchain games. The design is hierarchical and modular, ensuring scalability and reusability across different game elements.

## Elements

### Definition

Elements in Shinigami represent distinct entities within a game, such as achievements, bonuses, or other game-specific units. Each element implements a unique trait, allowing them to be uniformly processed within the same workflow.

### Responsibility

Handle specific game logic or intrinsic data associated with their type. Elements ensure consistency and facilitate streamlined operations within the game's ecosystem.

## Types

### Definition

Types encompass enumerators or custom types defining various states or functional intentions within the game. Examples include roles, items, actions, etc.

### Responsibility

Serve as entry points for associated elements, directing workflows to the appropriate logic based on the type. For instance, the Item type provides entry points for fundamental items like swords, potions, shields, etc.

## Models

### Definition

Models are entities with persistence in the game world, stored onchain and utilized across different transactions.

### Responsibility

Implement logic to manipulate and interact with stored data. Models encapsulate data management and ensure integrity during transactions.

## Components

### Definition

Components execute logic to manipulate different models within a cohesive workflow. They play a crucial role in verifying and maintaining overall coherence during player operations.

### Responsibility

Handle operations that involve multiple models, ensuring validations and updates are performed according to game rules and player actions.

## Systems

### Definition

Systems represent game modes, where each mode can utilize specific components with predefined configurations. For example, a game might have different systems like Standard using a default deck and Tutorial using an example deck.

### Responsibility

Manage game modes and configurations, allowing players to choose between different gameplay setups through the client interface.

## Helpers

### Definition

Helpers are reusable implementations that encapsulate common logic without game data. Examples include packers for packing/unpacking mechanisms, solvers for resolving game situations or either a battle for handling army fights.

### Responsibility

Provide utility functions to streamline repetitive tasks, ensuring code efficiency and reducing redundancy in complex game logic.

## Contributing

To contribute to the Shinigami framework, familiarize yourself with the outlined components and their responsibilities. Start by defining types and elements, progress to creating models and components, and extend to systems as needed for game modes. This structured approach ensures consistency and efficiency in developing fully onchain games on Starknet.
