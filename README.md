# LibGit2 Binding for Team Developer (SqlWindows)

This project provides a language binding for **LibGit2**, making it possible to integrate Git functionality into **Team Developer (TD)** applications, also known as **SqlWindows**. It enables TD developers to leverage the full power of Git directly from their TD projects using a simple and intuitive API.

## What is LibGit2?

**LibGit2** is a powerful, open-source library for interacting with Git repositories. It provides a C-based API for managing Git repositories, including features such as:

- **Cloning repositories**
- **Committing changes**
- **Creating and managing branches**
- **Merging branches**
- **Fetching and pulling from remotes**
- **Managing tags**

LibGit2 is used by popular Git clients such as **GitHub Desktop** and **GitLab**. It provides a lightweight and flexible way to work with Git in low-level environments or applications where command-line Git is not feasible.
More info on LibGit2 can be found here:

https://libgit2.org/

**LibGit2** is a standalone library that implements Git functionality in a C-based API, and it does not depend on an external Git installation. You can use LibGit2 in your applications without having Git installed on your system.

All Git operations (like cloning, committing, branching, etc.) are handled internally by LibGit2, so it provides the necessary functionality without requiring the Git command-line tool.

## What Can This TD Binding Do?

This binding enables Team Developer applications to:

- **Initialize and open repositories** within your TD applications.
- **Clone remote repositories** to local directories.
- **Perform Git operations** such as committing, ~~pulling, pushing, branching, and more.~~
- **Work with Git references**, ~~branches, and tags programmatically.~~

(Strikethrough is work in progress)

## Supported TD versions

The library is for TD 5.1 and up (32bit).
For older ANSI versions, backport the library and replace all calls to SalGetBufferLength/SalSetBufferLength to SalStrGetBufferLength/SalStrSetBufferLength.

## Usage

To use this binding, simply include the provided **LibGit2TD.apl** library in your TD project. The following features are available:

- **Repository Management**: Create, open, and clone Git repositories.
- **Committing**: Create commits to save your changes in the Git history.
- (Work in progress) **Branching**: List, create, and switch between branches.
- (Work in progress) **Remote Operations**: Fetch, pull, and push changes to/from remotes.
- (Work in progress) **Tagging**: Create and list tags within a repository.

### Example

Here’s an example of how you can clone a repository within your TD application using LibGit2TD:

```sqlwindows
// Pseudo-code in TD to clone a repository

Set bOk = wuGit.GIT_libgit2_init( nRet )
Set bOk = wuGit.GIT_clone( "https://github.com/TD-Community/WinAPI_Declarations.git", "c:\\temp\\myrepo", nRepoPtr, nRet )

```

## Installation

1. Download and include the **LibGit2 binding** library **LibGit2TD.apl** in your TD project.
2. Ensure that you have the **LibGit2TD.dll** library installed. Normally placed within the application runtime folder.
3. Start using Git commands within your TD environment.

## Requirements

- **Team Developer**: This binding is designed to be used within **Team Developer (SqlWindows)** version 5.1 and up.
- **LibGit2TD.dll**: You need to have this installed on your system, as this binding interacts directly with the library.
- **LibGit2TD.apl**: Include library to be added to your projects.

## Contribution

Feel free to contribute to this project by submitting issues or pull requests. We welcome enhancements, bug fixes, and feature requests.

## License

This project is licensed under the [MIT License](LICENSE).

---

## TD Community Forum
Join the TD Community Forum for everything related to Gupta Team Developer for related questions, answers and info.

https://forum.tdcommunity.net

If you like this project and want to enhance/improve it please do so.
Any help is appreciated. Changes to this project can be done by pull requests.
Like to be an official contributor, contact me to be added as contributor of this project.

Find me as Dave Rabelink on the forum mentioned above.
