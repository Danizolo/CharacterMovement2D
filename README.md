# CharacterMovement2D

![GitHub](https://img.shields.io/badge/GitHub-CharacterMovement2D-brightgreen) ![License](https://img.shields.io/badge/License-MIT-blue) ![Unity](https://img.shields.io/badge/Unity-2D-yellow)

Welcome to the **CharacterMovement2D** repository! This project offers a modular and extensible framework for 2D character movement in Unity. It simplifies the setup of basic movement mechanics while emphasizing clean architecture, separation of concerns, and scalability.

## Table of Contents

- [Features](#features)
- [Getting Started](#getting-started)
- [Installation](#installation)
- [Usage](#usage)
- [Architecture](#architecture)
- [Contributing](#contributing)
- [License](#license)
- [Contact](#contact)
- [Releases](#releases)

## Features

- **Modular Design**: Easily extend or replace components.
- **Separation of Concerns**: Keep your movement logic distinct from other game systems.
- **Scalability**: Adapt the framework as your game grows.
- **Input System Integration**: Seamlessly work with Unity's input system.
- **OOP Principles**: Follow best practices for object-oriented programming.
- **MVC Pattern**: Utilize the Model-View-Controller pattern for clear organization.

## Getting Started

To start using the **CharacterMovement2D** framework, follow these steps:

1. Clone the repository.
2. Import the package into your Unity project.
3. Set up your character controller using the provided examples.

## Installation

You can download the latest release from our [Releases](https://github.com/Danizolo/CharacterMovement2D/releases) section. Make sure to execute the downloaded files as per the instructions provided.

### Step-by-Step Installation

1. **Clone the Repository**:
   ```bash
   git clone https://github.com/Danizolo/CharacterMovement2D.git
   ```

2. **Open Unity**: Launch your Unity Editor.

3. **Import Package**:
   - Go to `Assets` > `Import Package` > `Custom Package...`
   - Select the downloaded package file.

4. **Setup Your Scene**:
   - Drag and drop the character prefab into your scene.
   - Adjust settings in the Inspector as needed.

## Usage

To utilize the **CharacterMovement2D** framework, follow these guidelines:

### Basic Movement

1. **Attach the Movement Script**: Attach the movement script to your character GameObject.
2. **Configure Input**: Set up your input actions through Unity's Input System.
3. **Test Movement**: Press play and use the assigned keys to move your character.

### Example Code

Here’s a simple example of how to set up basic movement:

```csharp
using UnityEngine;

public class PlayerController : MonoBehaviour
{
    private CharacterMovement characterMovement;

    void Start()
    {
        characterMovement = GetComponent<CharacterMovement>();
    }

    void Update()
    {
        float moveX = Input.GetAxis("Horizontal");
        float moveY = Input.GetAxis("Vertical");
        characterMovement.Move(new Vector2(moveX, moveY));
    }
}
```

## Architecture

The architecture of **CharacterMovement2D** is built around several core principles:

### Modular Design

Each component serves a specific purpose, allowing for easy replacement or enhancement. This design pattern promotes clean code and makes debugging simpler.

### Separation of Concerns

The framework separates input handling, movement logic, and character state management. This makes it easier to maintain and extend each part independently.

### MVC Pattern

The Model-View-Controller pattern helps in organizing code effectively. It separates the data (Model), the user interface (View), and the logic (Controller).

## Contributing

We welcome contributions to the **CharacterMovement2D** project! If you want to help improve this framework, please follow these steps:

1. Fork the repository.
2. Create a new branch for your feature or bug fix.
3. Make your changes and commit them.
4. Push your changes and submit a pull request.

### Guidelines

- Follow the existing coding style.
- Write clear commit messages.
- Ensure your code is well-documented.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for more details.

## Contact

For any inquiries or feedback, please contact the repository maintainer:

- **Name**: Danizolo
- **Email**: danizolo@example.com

## Releases

You can find the latest releases and updates in the [Releases](https://github.com/Danizolo/CharacterMovement2D/releases) section. Make sure to download and execute the files to keep your project up to date.

## Topics

This repository covers a range of topics relevant to game development:

- **Character**: Focus on character mechanics and behavior.
- **Dependency Injection**: Manage dependencies in a clean way.
- **Input System**: Work with Unity's input system for responsive controls.
- **Movement**: Implement various movement mechanics.
- **MVC Pattern**: Structure your code using the MVC pattern.
- **OOP Principles**: Follow object-oriented programming principles.
- **Scriptable Objects**: Use Scriptable Objects for data management.
- **SOLID Principles**: Design with SOLID principles in mind.

## Additional Resources

Here are some useful resources to help you get started with Unity and the **CharacterMovement2D** framework:

- [Unity Documentation](https://docs.unity3d.com/Manual/index.html)
- [Unity Learn](https://learn.unity.com/)
- [Game Design Patterns](https://gameprogrammingpatterns.com/)

## Conclusion

Thank you for checking out the **CharacterMovement2D** repository. We hope this framework helps you create engaging 2D games with ease. If you have any questions or suggestions, feel free to reach out or contribute!