# 🫙 DevContainers
**DevContainers** is a free and open-source directory of different VSCode `.devcontainer` configurations to start developing projects **fast**.

In VSCode you can develop inside a Docker Container and, this way, ensure your code will work on any deployment as well as across multiple systems if you're working in a team. If you want to learn more about this you can visit the [VSCode documentation](https://code.visualstudio.com/docs/devcontainers/containers).

<details open>
<summary>Table of Contents</summary>

- [Getting Started](#getting-started)
  - [Structure](#structure)
  - [Configuration](#configuration)
  - [Dependencies](#dependencies)
  - [Starting the dev container](#starting-the-dev-container)
- [Frequently Asked Questions](#frequently-asked-questions)
- [Contributing](#contributing)
- [License](#license)

</details>


# Getting Started

Every devcontainer is configurable, there are some base extensions that might be useful for you but you are free to remove or add the ones you need.

## Structure

Every folder in this repository is meant for a different system. These are the current available ones:

- `.devcontainer.django_postgres_redis` - django with a postgres and a redis database
- `.devcontainer.node` - Vite, React, Astro...

## Configuration

Inside every devcontainer directory you will find a `devcontainer.json` file. Inside, you can modify things such as the name of the devcontainer, the action on shutdown, or VSCode extensions and settings.

Everything is commented in there so it's easy to add or remove stuff as needed.

Every devcontainer folder has a README file where you can find more information.

## Dependencies

- Docker installed in your system
- The Docker extension in VSCode
- The Dev Containers extension in VSCode

## Starting the dev container

1. Copy the devcontainer folder you want to use into the root directory of your project
2. Rename the folder to `.devcontainer`
3. In VSCode, open the command pallete and run **"Dev Containers: Reopen in Container"**
4. You're good to go!

# Frequently Asked Questions

## My dev container is suuuper slow!

In windows, dev containers are quite slow due to the mounting system of the devcontainer to your storage. In Windows, it is much preferable to run the dev containers in WSL.You can follow [these instructions](https://code.visualstudio.com/blogs/2020/07/01/containers-wsl)

# Contributing

If you have any idea, suggestions or find any bugs, feel free to open a discussion, an issue or create a pull request. That would be very useful for all of us and we would be happy to listen and take action.

# Liscense

**DevConainers** is licensed under the MIT license — see the [LICENSE](./LICENSE.md) file for details.