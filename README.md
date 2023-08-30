# UnchainedCore - RP Intensive Gameplay Framework

UnchainedCore is a versatile framework designed to enhance FiveM server development, specifically tailored for RP-intensive gameplay. With a strong focus on performance optimization, UnchainedCore empowers developers to create immersive role-playing experiences while maintaining a stable and optimized server environment.

## Features

- **Performance Optimization**: UnchainedCore is built with performance in mind. Utilize its efficient architecture to minimize resource consumption and provide players with a smooth and enjoyable RP experience.

- **Modular Structure**: The framework is organized into distinct client, server, and shared modules, ensuring clear separation and streamlined development of your RP features.

- **Shared Configuration**: Centralize your configuration settings in the shared directory, ensuring consistency between the client and server sides of your resource.

- **RP-Centric Enhancements**: UnchainedCore comes with a suite of tools and utilities aimed at enhancing RP gameplay, including seamless emote systems, in-character chat functionalities, and more.

- **Extensive Documentation**: Get started quickly with comprehensive documentation, including installation instructions, API references, and usage examples.

## Getting Started

To incorporate UnchainedCore into your FiveM server, follow these steps:

1. **Clone the Repository**: Clone this repository to your server's resources directory.

2. **Configuration**: Customize the framework's configuration files according to your server's needs. Modify the `shared/config.lua`, `client/config.lua`, and `server/config.lua` files to set up your RP rules, environment settings, and more.

3. **Resource Manifest**: In your resource's `fxmanifest.lua` file, specify the dependencies and include UnchainedCore in your resource stack:

```lua
fx_version 'cerulean'
game 'gta5'

-- Define your resource
name 'your-resource-name'
description 'Your resource description'
author 'Your name'

-- Define dependencies
dependencies {
    'unchainedcore' -- Add UnchainedCore as a dependency
}

-- Specify the entry files
client_script 'client/main.lua'
server_script 'server/main.lua'
shared_script 'shared/config.lua'
