# Versioning

While many developers and vendors use the term in different contexts, versioning most often applies to operating systems, software artifacts and web services.

Software versioning helps developers, project managers, product managers and consumers keep track or identify the state a software product or package is in with a unique name and/or a number, thus providing a universal way of understanding the release process.

## Table of Contents

## Introduction

In the world of software management there exists a dreaded place called “dependency hell.” The bigger your system grows and the more packages you integrate into your software, the more likely you are to find yourself, one day, in this pit of despair.

In systems with many dependencies, releasing new package versions can quickly become a nightmare. If the dependency specifications are too tight, you are in danger of version lock (the inability to upgrade a package without having to release new versions of every dependent package). If dependencies are specified too loosely, you will inevitably be bitten by version promiscuity (assuming compatibility with more future versions than is reasonable). Dependency hell is where you are when version lock and/or version promiscuity prevent you from easily and safely moving your project forward.

As a solution to this problem, we propose a simple set of rules and requirements that dictate how version numbers are assigned and incremented. These rules are based on but not necessarily limited to pre-existing widespread common practices in use in both closed and open-source software. For this system to work, you first need to declare a public API. This may consist of documentation or be enforced by the code itself. Regardless, it is important that this API be clear and precise. Once you identify your public API, you communicate changes to it with specific increments to your version number. Consider a version format of X.Y.Z (Major.Minor.Patch). Bug fixes not affecting the API increment the patch version, backward compatible API additions/changes increment the minor version, and backward incompatible API changes increment the major version.

We call this system “Semantic Versioning.” Under this scheme, version numbers and the way they change convey meaning about the underlying code and what has been modified from one version to the next.

-----------
This Documentation resource like all my other documentations is made up of research study notes based curated informational resources from books, articles and other useful online content with the intention of informing myself and making this rich material readily available for anyone else having a hard time finding this kind of information.

---------------

## What is Versioning?

Versioning is the creation and management of multiple product releases, all of which have the same general function, but are improved, upgraded or customized.

For example, say our fictional company **Intellus Business Solutions** was developing a software product for release, it can assign unique names or specific numerical identifiers to ongoing series of this product releases, such as _intellus v.1, v.1.1,---n, v.2.0, 2.1,---n._

The numbers represent different versions of the same software product or application, and the numbers assigned increase to correspond to the latest development and releases.

Subsequent releases of the same product can also be assigned numerical identifiers consisting of two or three numbers separated by periods.

- The first number, called the major number, is increased when there are significant improvements or changes in functionality. For example, when Intellus v.1 makes major upgrades, from its erstwhile Intellus 1 to Intellus 2, intellus v.1, changes to v.2.
- The second number, called the minor number, is incremented when there are minor feature changes or notable fixes. Intellus v.1 can indicate minor changes were made to it by indicating the release as, Intellus v.1.1.
- The third number, if it exists, is called the revision number and is added or increased when minor bugs are eliminated. For example, Intellus v.1.1.2 would show that bug fixes were made to the previous version.

To sum this up, given a version number MAJOR.MINOR.PATCH, increment the:

1. MAJOR version when you make incompatible API changes
2. MINOR version when you add functionality in a backward compatible manner
3. PATCH version when you make backward compatible bug fixes

Additional labels for pre-release and build metadata are available as extensions to the MAJOR.MINOR.PATCH format.

In software engineering , versioning allows software development teams keep track of major & minor changes they make to the software project code, which may include new functions, features or bugfixes. It can also be an internal practice used to make it easier for developers to keep track of code evolution.

## Semantic Versioning (SemVer)

Semantic Versioning, often abbreviated as SemVer, is a widely adopted versioning scheme in the software development industry proposed by Tom Preston-Werner in 2013 for software release version control with the aims of conveying meaning about the underlying changes in a release through version numbers.

 Semantic versioning, or SemVer, is often used as a versioning framework for applications, plugins, extensions and different software objects. 

SemVer comprises three parts, X.Y.Z, where X, Y and Z are non-negative integers. This means that the primary or major version is X, and the minor version is Y. Bug fixes and patches are called version Z. So, it always takes the form of X.Y.Z, or major.minor.patch. For example, in SemVer 1.8.0, 1 indicates the major version, 8 the minor version, and 0 the bug fixes or patches.

 SemVer consists of three components: major, minor, and patch versions, represented as MAJOR.MINOR.PATCH.

- Major Version (MAJOR): This digit is incremented when incompatible changes are introduced in the software. It signifies that there are breaking changes in the codebase, and developers should expect potential backward compatibility issues.
- Minor Version (MINOR): When new features or enhancements are added in a backward-compatible manner, the minor version is incremented. Developers can safely update to a new minor version without worrying about breaking changes.
- Patch Version (PATCH): The patch version is incremented for backward-compatible bug fixes and minor improvements that do not introduce new features or breaking changes.

## Benefits of Semantic Versioning

- Predictability: By adhering to SemVer, developers and users of a library or package can anticipate the impact of an update. They can quickly assess whether an upgrade is safe or might require adjustments to their codebase.
- Dependency Management: Package managers like npm, Composer, and pip rely on Semantic Versioning to resolve and install compatible dependencies automatically. This helps maintain consistency in your project's ecosystem.
- Communication: SemVer serves as a communication tool between developers. When a new version is released, the change in version number provides immediate insight into the nature of the update.
- You can keep track of every transition in the software development phase. Versioning the software ensures you that every team member or user can keep track of what has been changed and when;
- Versioning can do the job of explaining to the developers what type of changes have taken place and the possible updates that should take place in the software;
- It helps to keep things clean and meaningful. So, other people who might be using your project as a dependency;
- SemVer lets you know which version of a product is no longer backward compatible.

## Using Semantic Versioning Effectively

- Start with Version 1.0.0: Every project should begin with version 1.0.0. This signifies that it's in its initial development phase.
- Increment Versions Mindfully: Major (MAJOR) for backward-incompatible changes.Minor (MINOR) for new features or enhancements.Patch (PATCH) for backward-compatible bug fixes.
- Use Pre-release and Build Metadata: SemVer allows for appending pre-release and build metadata to versions. For example, you can have versions like 1.0.0-alpha or 1.0.0+20231006.
- Document Changes: Maintain a changelog or release notes to document the changes made in each version. This helps users understand what has been added, fixed, or changed.
- Test and Automate: Implement automated testing and continuous integration to ensure that changes introduced in different versions do not break existing functionality.

## Other existent versioning schemes

- CalVer this scheme relies on the date of the release. It is not as specific as the SemVer scheme but is used by projects such as Pip the Python package manager and Ubuntu
- Python Versioning Scheme is a scheme defined to identify distributions of Python. The scheme uses five segments called epoch, release, pre-release, post-release, and development
- Named Versions some projects opt to name their releases with a unique name. For example, Android has an interesting collection of version names that started off with Cupcake, Donut, and Eclair!
- Spring Project Version Scheme — this is a common method in Spring Framework and Spring Boot projects and expands on SemVer with some additional labels such as RC (release candidates) and BUILD-SNAPSHOT ( for a development release)

## Git & GitHub

- **Git** is a version control system for tracking changes in source code during software development. It helps coordinate work among programmers. Git is an open source software that's licensed. It's installed locally on a computer.

- **GitHub** is an online service that provides a place to host source code as well as contribute and collaborate. It lets people work together on projects from anywhere. GitHub is a service, not a software. It offers free, professional, and enterprise accounts.

You can use Git without using GitHub, but you cannot use GitHub without using Git. Typically, People work with repositories in GitHub. A repository is like a folder for your project. You can have multiple public and private repositories in GitHub. Repositories can contain files, images, videos, spreadsheets, and data sets. GitHub provides the revision history for all files in a repository.

In general, in GitHub you can:

- Host your own open source project. To do this, you create an online repository and add files.
- Contribute to an existing open source project that’s public. To do this, you access a copy of the project’s repository, make updates, and request a review of the changes to you want to contribute.



### 𝗛𝗼𝘄 𝗚𝗜𝗧 𝗪𝗼𝗿𝗸𝘀?

Git is a distributed version control tool that facilitates monitoring changes made to your code over time. Git makes it simple to track changes to your codebase and collaborate on projects with others. It was authored by Linus Torvalds in 2005 for developing the 𝗟𝗶𝗻𝘂𝘅 𝗸𝗲𝗿𝗻𝗲𝗹, with other kernel developers contributing to its initial development.

It enables us to 𝘁𝗿𝗮𝗰𝗸 𝗰𝗵𝗮𝗻𝗴𝗲𝘀 𝗶𝗻 𝗼𝘂𝗿 𝗰𝗼𝗱𝗲 𝗮𝗻𝗱 𝗰𝗼𝗹𝗹𝗮𝗯𝗼𝗿𝗮𝘁𝗲 𝘄𝗶𝘁𝗵 𝗼𝘁𝗵𝗲𝗿𝘀 others by working on a different part of a codebase. When we say distributed, we may think we have code in two locations: a remote server and a local one, but the story is a bit more complex. 

Git has three local storages: a working directory, a staging area, and a local repository.

𝟭. 𝗪𝗼𝗿𝗸𝗶𝗻𝗴 𝗗𝗶𝗿𝗲𝗰𝘁𝗼𝗿𝘆 - This is where you work and your files live (also called "untracked"). All file changes here will be marked, and if they are not saved to GIT, you will lose them. The reason is that GIT is not aware of those files. 

𝟮. 𝗦𝘁𝗮𝗴𝗶𝗻𝗴 𝗔𝗿𝗲𝗮 - When you save your changes with git add, GIT will start tracking and saving your changes with files. These changes are stored in the .git directory. Then, files are moved from the Working Directory to the Staging Area. Still, if you change these files, GIT will not know about them; you need to tell GIT to notice those changes. 

𝟯. 𝗟𝗼𝗰𝗮𝗹 𝗥𝗲𝗽𝗼𝘀𝗶𝘁𝗼𝗿𝘆 - It is the area where everything is saved (commits) in the .git directory. When you want to move your files from the Staging Area to the Local Repository, you can use the git commit command. After this, your Staging area will be empty. If you want to see what is in the Local repository, try git log. 

Some basic 𝗚𝗜𝗧 𝗰𝗼𝗺𝗺𝗮𝗻𝗱𝘀 are:

🔹 𝗴𝗶𝘁 𝗶𝗻𝗶𝘁 -> Create a new git repo in the directory
🔹 𝗴𝗶𝘁 𝗯𝗿𝗮𝗻𝗰𝗵 -> Create a new local branch 
🔹 𝗴𝗶𝘁 𝗰𝗵𝗲𝗰𝗸𝗼𝘂𝘁 -> Switch branches
🔹 𝗴𝗶𝘁 𝗮𝗱𝗱 -> Add a new file to your staging area
🔹 𝗴𝗶𝘁 𝗰𝗼𝗺𝗺𝗶𝘁 -> Adds staged changes to your local repository
🔹 𝗴𝗶𝘁 𝗽𝘂𝗹𝗹 -> pull code from your remote repo to your local directory
🔹 𝗴𝗶𝘁 𝗽𝘂𝘀𝗵 -> Push local repository changes to your remote repo
🔹 𝗴𝗶𝘁 𝘀𝘁𝗮𝘁𝘂𝘀 -> Show which files are being tracked (and untracked)
🔹 𝗴𝗶𝘁 𝗱𝗶𝗳𝗳 -> See the actual difference in code between your Working Directory and your Staging Area

In addition to GIT commands, you can try some popular 𝗚𝗜𝗧 𝘁𝗼𝗼𝗹𝘀: GitHub Desktop, SourceTree, TortoiseGit, Git Extensions, GitKraken, SmartGit, Tower, etc.

Check the GIT command cheat sheet in the comments.


### Basic GIT Commands

- ``git int`` - Initialise a new git repository.
- ``git clone`` - Clone an exsisting Git Repository to your local machine.
- ``git add`` - Stages changes to a file for the next commit.
- ``git commit`` - Commits staged changes to the repository.
- ``git reset`` - Unstage changes or resets the working directory to a previous commit.
- ``git status`` - Shows the status of a working directory.
- ``git log`` - Shows the history of commits to the repository.
- ``git branch`` - Creates,lists, or switches branches.
- ``git merge`` - Merges changes from one branch into another.
- ``git pull`` - Fetches and merges changes from the remote repository.
- ``git push`` - Pushes changes from the local repository to the remote repository.

## **𝐆𝐢𝐭𝐇𝐮𝐛 𝐂𝐡𝐞𝐚𝐭𝐬𝐡𝐞𝐞𝐭**

### 𝐑𝐞𝐩𝐨𝐬𝐢𝐭𝐨𝐫𝐲 𝐁𝐚𝐬𝐢𝐜𝐬

- Command to **Clone a Repository**:

 ```cmd
    git clone <repository_url>
```

- Command to **Initialize a Repository**:

```cmd
   git init
```

### 𝐖𝐨𝐫𝐤𝐢𝐧𝐠 𝐰𝐢𝐭𝐡 𝐁𝐫𝐚𝐧𝐜𝐡𝐞𝐬

- Command to **Create a New Branch**:

```cmd
   git branch <branch_name>
```

- Command to **Switch to a Branch**:

```cmd
   git checkout <branch_name>
```

- Command to **Create and Switch to a New Branch:**

```cmd
   git checkout -b <new_branch_name>
```

- Command to **List Branches**:

```cmd
   git branch
```

### 𝐂𝐨𝐦𝐦𝐢𝐭𝐭𝐢𝐧𝐠 𝐂𝐡𝐚𝐧𝐠𝐞𝐬

- Command to **Stage Changes**:

```cmd
   git add <file_name>
```

- Command to **Stage All Changes**:

```cmd
   git add .
```

- Command to **Commit Changes**:

```cmd
   git commit -m "Commit message"
```

### 𝐏𝐮𝐥𝐥𝐢𝐧𝐠 𝐚𝐧𝐝 𝐏𝐮𝐬𝐡𝐢𝐧𝐠

- Command to **Pull Changes from Remote**:

```cmd
   git pull origin <branch_name>
```

- Command to **Push Changes to Remote**:

```cmd
 git push origin <branch_name>
```

### 𝐌𝐞𝐫𝐠𝐢𝐧𝐠 𝐂𝐡𝐚𝐧𝐠𝐞𝐬

- Command to **Merge Branch into Current Branch**:

```cmd
   git merge <branch_name>
```

### 𝐖𝐨𝐫𝐤𝐢𝐧𝐠 𝐰𝐢𝐭𝐡 𝐑𝐞𝐦𝐨𝐭𝐞𝐬

- Command to **Add a Remote Repository**:

```cmd
   git remote add <remote_name> <repository_url>
```

- Command to **List Remote Repositories**:

```cmd
   git remote -v
```

### 𝐇𝐚𝐧𝐝𝐥𝐢𝐧𝐠 𝐂𝐨𝐧𝐟𝐥𝐢𝐜𝐭𝐬

- Command to **Check for Conflicts**:

```cmd
   git diff
```

- Command to **Resolve Conflicts and Continue Merge**:

```cmd
   git add <file_name>
   git merge --continue
```

### 𝐆𝐢𝐭𝐇𝐮𝐛 𝐀𝐜𝐭𝐢𝐨𝐧𝐬

- Command for **Workflow Syntax Checking**:

```cmd
   git pull origin <branch_name>
   git push origin <branch_name>
```

### 𝐌𝐢𝐬𝐜𝐞𝐥𝐥𝐚𝐧𝐞𝐨𝐮𝐬

- Command to **Check Git Status**:

```cmd
   git status
```

- Command to **View Commit History**:

```cmd
   git log
```

- Command to **Ignore Files (Add to `.gitignore`)**:

```cmd
   echo "<file_name>" >> .gitignore
```

## Conclusions

There are many different ways of versioning software products and artifacts with one of the most popular schemes being semantic versioning.

Semantic Versioning, often abbreviated as SemVer, is a versioning scheme for software that aims to convey meaning about the underlying changes in a release through version numbers.

SemVer is a popular versioning scheme that is used by a vast amount of open-source projects to communicate the changes included in a version release. As developers, it’s important for us to understand how to use SemVer in our own projects and also how to interpret a specific version change.

Semantic Versioning is a powerful tool for versioning software that fosters predictability, ease of communication, and efficient dependency management. By following the guidelines of SemVer, developers can maintain a well-structured versioning system that benefits both creators and consumers of software packages.

## References & Resources

- [Semantic Versioning 2.0.0](https://semver.org/)
- [Gentle introduction to semantic versioning](https://medium.com/@jteodoro/gently-introduction-to-semantic-versioning-f4e015956c8c)
- [A Guide to Semantic Versioning](https://www.baeldung.com/cs/semantic-versioning)
- [versioning](https://www.techtarget.com/searchsoftwarequality/definition/versioning)
- [Automating Versioning and Releases Using Semantic Release](https://medium.com/agoda-engineering/automating-versioning-and-releases-using-semantic-release-6ed355ede742)
- [GitHub Pages](https://pages.github.com/)
- [Netlify](https://www.netlify.com/)
- [How to merge two or multiple git repositories into one](https://medium.com/altcampus/how-to-merge-two-or-multiple-git-repositories-into-one-9f8a5209913f)
- [combining-git-repositories.md](https://gist.github.com/msrose/2feacb303035d11d2d05)
- [Git in 15 Minutes](https://youtu.be/USjZcfj8yxE?si=Bhnn6xHBbxSEfc4H)
- [GitHub in 20 Minutes](https://youtu.be/nhNq2kIvi9s?si=i_4skWMnHdxBwHSK)
## Keywords

``Versioning``, ``Version Control``, ``SemVer``, ``Semantic Version Control``, ``Git``, ``Git Commands``, ``GitHub``, ``GitHub Actions``
