# [Project Template]

## Software Kit

![Blender](https://img.shields.io/badge/blender-%23F5792A.svg?style=for-the-badge&logo=blender&logoColor=white)
![.Net](https://img.shields.io/badge/.NET-5C2D91?style=for-the-badge&logo=.net&logoColor=white)
![C#](https://img.shields.io/badge/c%23-%23239120.svg?style=for-the-badge&logo=c-sharp&logoColor=white)
![Unity](https://img.shields.io/badge/unity-%23000000.svg?style=for-the-badge&logo=unity&logoColor=white)
![Visual Studio Code](https://img.shields.io/badge/Visual%20Studio%20Code-0078d7.svg?style=for-the-badge&logo=visual-studio-code&logoColor=white)
![Vim](https://img.shields.io/badge/VIM-%2311AB00.svg?style=for-the-badge&logo=vim&logoColor=white)
![Audacity](https://img.shields.io/badge/Audacity-0000CC?style=for-the-badge&logo=audacity&logoColor=white)
![Git](https://img.shields.io/badge/git-%23F05033.svg?style=for-the-badge&logo=git&logoColor=white)
![Gimp Gnu Image Manipulation Program](https://img.shields.io/badge/Gimp-657D8B?style=for-the-badge&logo=gimp&logoColor=FFFFFF)
![Aseprite](https://img.shields.io/badge/Aseprite-FFFFFF?style=for-the-badge&logo=Aseprite&logoColor=#7D929E)

## Requirements

### Software

| Name  | Version        |                        Link                        |
| :---- | :------------- | :------------------------------------------------: |
| Unity | 2021.3.0f1 LTS | [Download](https://unity3d.com/get-unity/download) |

### Reading

| Source              |                          Link                          |
| :------------------ | :----------------------------------------------------: |
| Unity Documentation |             [View](https://docs.unity.com)             |
| C# Documentation    | [View](https://docs.microsoft.com/en-us/dotnet/csharp) |

---

## Folder Structure

```
|-- Assets
      |-- Animations
      |-- Editor
      |-- Media
      |   |-- Audio
      |   |-- Video
      |-- Sprites
      |-- Models
      |-- ScriptTemplates
      |-- Materials
      |-- Shaders
      |-- Plugins
      |-- Fonts
      |-- Prefabs
      |   |-- Characters
      |   |-- Weapons
      |   |-- Other
      |-- Scenes
      |   |-- Levels
      |-- Scripts
      |   |-- Editor
      |   |-- Scriptables
      |   |-- Managers
      |   |-- Utilities
      |   |-- Units
      |   |-- Other
      |-- _ExternalAssets
            |-- Media
            |   |-- Audio
            |   |-- Video
            |-- Sprites
            |-- Models
            |-- Materials
            |-- Shaders
            |-- Fonts
            |-- Scripts
```

| Folder              | Description                                                                                                           |
| :------------------ | :-------------------------------------------------------------------------------------------------------------------- |
| Animations          | Store all animations here.                                                                                            |
| Editor              | Store all editor specific files here.                                                                                 |
| Media               | Store all audio and video files here.                                                                                 |
| Sprites             | Store all 2D sprites here.                                                                                            |
| Models              | Store all 3D models here.                                                                                             |
| Materials           | Store all materials here.                                                                                             |
| Shaders             | Store all shaders here.                                                                                               |
| Plugins             | Store any plugins you use here.                                                                                       |
| Fonts               | Store all font files here.                                                                                            |
| Scenes              | Store all scenes here.                                                                                                |
| Prefabs             | Store all prefabs here.                                                                                               |
| Scripts             | Store all scripts here.                                                                                               |
| Scripts/Editor      | For Editor specific scripts.                                                                                          |
| Scripts/Scriptables | For scripts meant to transport, store or transform data, like ScriptableObjects.                                      |
| Scripts/Managers    | For singleton type scripts.                                                                                           |
| Scripts/Utilities   | For utilty scripts used across the project.                                                                           |
| Scripts/Units       | For implementations of scripts or other resources.                                                                    |
| \_ExternalAssets    | This is a reflection of the Assets folder, but meant for external assets you want to keep seperate from your project. |

---

## Conventions

| Name                        | Rule                                                                             | Example                            |
| :-------------------------- | :------------------------------------------------------------------------------- | :--------------------------------- |
| Private Variables           | Use camel case and start with an underscore.                                     | `private int _myPrivateVariable;`  |
| Local Variables             | Use camel case.                                                                  | `var myLocalVariable = 4;`         |
| Public Variables            | Use pascal case.                                                                 | `public int MyPublicVariable;`     |
| Folders                     | Use pascal case.                                                                 | FolderNameHere                     |
| Function Naming             | Use pascal case.                                                                 | `public int MyFunction();`         |
| Variable Declaration        | Always use `var` to create variables.                                            | `var myVariable = "use var";`      |
| Max Parameters              | A method should not have more than 6 parameters.                                 | -                                  |
| No magic numbers or strings | Do not use magic variables, rather define them as constant in a single location. | -                                  |
| Function Calling            | Include the parameter name when calling a function.                              | `myFunction(id: 1, name: "Fred");` |

---

## Commit Structure

Please follow the Conventional Commits standards as well as squashing your commits into a single commit.

Specification can be found at [www.conventionalcommits.org](https://www.conventionalcommits.org/en).

How to squash commits: [https://www.git-tower.com/learn/git/faq/git-squash](https://www.git-tower.com/learn/git/faq/git-squash)

Commits should be in the following form: **type[optional scope]: description**. Examples include:

> feat: allow provided config object to extend other configs

> feat(api)!: send an email to the customer when a product is shipped

> docs: correct spelling of CHANGELOG

|       Type        | Title                    | Emoji | Release | Description                                                                                                 |
| :---------------: | ------------------------ | :---: | :-----: | ----------------------------------------------------------------------------------------------------------- |
|      `feat`       | Features                 |  ✨   | `minor` | A new feature                                                                                               |
|    `refactor`     | Code Refactoring         |  📦   | `patch` | A code change that neither fixes a bug nor adds a feature                                                   |
|      `perf`       | Performance Improvements |  🚀   | `patch` | A code change that improves performance                                                                     |
|       `fix`       | Bug Fixes                |  🐛   | `patch` | A bug Fix                                                                                                   |
|      `chore`      | Chores                   |   ♻   | `patch` | Other changes that don't modify src or test files                                                           |
|     `revert`      | Reverts                  |   🗑   | `patch` | Reverts a previous commit                                                                                   |
|      `docs`       | Documentation            |  📚   | `patch` | Documentation only changes                                                                                  |
|      `style`      | Styles                   |  💎   |    -    | Changes that do not affect the meaning of the code (white-space, formatting, missing semi-colons, etc)      |
|      `test`       | Tests                    |  🚨   |    -    | Adding missing tests or correcting existing tests                                                           |
|      `build`      | Builds                   |   🛠   | `patch` | Changes that affect the build system or external dependencies (example scopes: gulp, broccoli, npm)         |
|       `ci`        | Continuous Integrations  |   ⚙   |    -    | Changes to our CI configuration files and scripts (example scopes: Travis, Circle, BrowserStack, SauceLabs) |
| `BREAKING CHANGE` | Breaking Change          |  💔   | `major` | When a breaking change occurs on the commit. Rather use the "!" operator in conjunction with a type.        |
