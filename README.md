# TD integration with Git

## What is LibGit2TD?

Here’s a sample `README.md` for your GitHub project that provides an overview of the language binding for **LibGit2** in **Team Developer (TD)** applications:

---

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

## What Can This Binding Do?

This binding enables Team Developer applications to:

- **Initialize and open repositories** within your TD applications.
- **Clone remote repositories** to local directories.
- **Perform Git operations** such as committing, pulling, pushing, branching, and more.
- **Work with Git references**, branches, and tags programmatically.

## Usage

To use this binding, simply include the provided **LibGit2TD.apl** library in your TD project. The following features are available:

- **Repository Management**: Create, open, and clone Git repositories.
- **Branching**: List, create, and switch between branches.
- **Committing**: Create commits to save your changes in the Git history.
- **Remote Operations**: Fetch, pull, and push changes to/from remotes.
- **Tagging**: Create and list tags within a repository.

### Example

Here’s an example of how you can clone a repository within your TD application:

```sqlwindows
// Pseudo-code in TD to clone a repository
Call GitCloneRepository(
    "https://github.com/your-repository.git",
    "C:\path\to\local\directory"
)
```

## Installation

1. Download and include the **LibGit2 binding** library **LibGit2TD.apl** in your TD project.
2. Ensure that you have the **LibGit2TD.dll** library installed. Normally placed within the application runtime folder.
3. Start using Git commands within your TD environment.

## Requirements

- **Team Developer**: This binding is designed to be used within **Team Developer (SqlWindows)**.
- **LibGit2TD.dll**: You need to have this installed on your system, as this binding interacts directly with the library.
- **LibGit2TD.apl**: Include library to be added to your projects.

## Contribution

Feel free to contribute to this project by submitting issues or pull requests. We welcome enhancements, bug fixes, and feature requests.

## License

This project is licensed under the [MIT License](LICENSE).

---

## TD Community Forum
Join the TD Community Forum for everything related to Gupta Team Developer for related questions, answers and info. Also for this NetHookTD project

https://forum.tdcommunity.net

If you like this project and want to enhance/improve it please do so.
Any help is appreciated. Changes to this project can be done by pull requests.
Like to be an official contributor, contact me to be added as contributor of this project.

Find me as Dave Rabelink on the forum mentioned above.
