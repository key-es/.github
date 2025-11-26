# Hi there 👋

<!--
Comments
🧙 Remember, you can do mighty things with the power of [Markdown](https://docs.github.com/github/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax)
-->

The key-es GitHub organisation is for internal sharing of reuse code.

The minimum requirement is that packages are supported for LabVIEW 2020 and higher.

# ☁️ Source Control

## 🛠️ Setup Source Control

Create a new repository on GitHub:
<img width="889" height="864" alt="image" src="https://github.com/user-attachments/assets/31513ce8-3e8a-43f7-99a3-2c4762c9352e" />

Using the command line, clone the repository:

`git clone git@github.com:user-name/repo-name.git`

Create a new LabVIEW project in this directory - this is where you will develop your package.

## 🌳 Branches

|Branch Name|Description|
|-----------|-----------|
|`main`|Release branch|
|`dev`|Development branch|
|`[issue-id]`|Development on a particular issue|


Create the `dev` branch on GitHub:
<img width="1479" height="649" alt="image" src="https://github.com/user-attachments/assets/7440bb70-9aaf-4e16-8319-4ed2fc7260f0" />


Pull down the new branch to your local copy from the command line:

`git pull`

Switch to the new `dev` branch:

`git switch dev`

Work on the `dev` or a specific `[issue-id]` branch. Once development is complete and unit tests have been passed, merge into `main`.

## ⁉️ Issues

## 💬 Conventional Commits


Conventional commits provide an easy set of rules to write an explicit commit history.

The commit message should be structured as follows:
```
<type>[optional scope]: <description>

[optional body]

[optional footer(s)]
```

Appending `!` to the commit `<type>` denotes a breaking change.

|Type|Description|
|---|---|
|`fix`|Patches an API or UI bug - this correlates to `PATCH` in Semantic Versioning|
|`feat`|Introduces, adjusts, or removes a new feature to the API or UI - this correlates to `MINOR` in Semantic Versioning|
|`refactor`|Rewrites or restructures code without altering API or UI behavior|
|`perf`|A type of `refactor` that specifically improves performance|
|`style`|Addresses code style (e.g., white-space, formatting, missing semi-colons) and does not affect application behavior|
|`test`|Adds missing tests or corrects existing ones|
|`docs`|Alters documentation e.g. update `README.md`|
|`build`|Changes to build-related components such as build tools, external dependencies, project version|
|`ops`|Changes to operational components like infrastructure, deployment, backup, recovery procedures|
|`chore`|Miscellaneous e.g. modifying `.gitignore`|

Resources:
- https://www.conventionalcommits.org/en/v1.0.0
- https://github.com/angular/angular/blob/22b96b9/CONTRIBUTING.md#-commit-message-guidelines
- https://gist.github.com/qoomon/5dfcdf8eec66a051ecd85625518cfd13

## ⭐ Releases

When the changes have been made and the package/module has been built and is ready for release, commit the project using the command line, referencing the release version number:

`git add .`

`git commit -m 'Release 1.0.0'`

Tag the commit. This tag marks the *exact* commit the package/module was built from:

`git tag -a 1.0.0 -m 'Release 1.0.0 - first release'`

`git push origin main --tags`

From GitHub, create a new release referencing this tag, update the release notes, and attach the `.vip` file.

<img width="1038" height="867" alt="image" src="https://github.com/user-attachments/assets/db0c7112-faaa-416e-be74-4e02205e0b4f" />



# 🔢 Versioning

When creating new packages/modules it is inevitable that changes and updates will be made. 

## Semantic Versioning 2.0.0

[Semantic Versioning 2.0.0](https://semver.org/) is the widely used, preferred formatting of version numbers. This is summarised below.

Given a version number MAJOR.MINOR.PATCH, increment the:
- MAJOR version when you make incompatible API changes
- MINOR version when you add functionality in a backward compatible manner
- PATCH version when you make backward compatible bug fixes
Additional labels for pre-release and build metadata are available as extensions to the MAJOR.MINOR.PATCH format.

If the MAJOR number is incremented, the MINOR and PATCH numbers are reset. Similarly, if the MINOR number is updated, the PATCH number is reset.

## VI Package Builder Versioning

The version number of a package can be set/updated in the VI Package Builder under the Basic > Build Information tab:

<img width="1033" height="790" alt="image" src="https://github.com/user-attachments/assets/4701d419-cd88-4b48-8d1f-c206b1824f95" />

The output filename will contain the version number by default (if it does not automatically update when the version number is changed, clicking the edit button, and then cancelling will update it). This can be seen in the Advanced > Package Filename tab:

<img width="1033" height="790" alt="image" src="https://github.com/user-attachments/assets/aff5cd08-73e9-4e3b-94e4-50011d2b49cf" />



# 🔗 Useful Resources

## Semantic Versioning
- https://semver.org/

## Conventional Commits
- https://www.conventionalcommits.org/en/v1.0.0
- https://github.com/angular/angular/blob/22b96b9/CONTRIBUTING.md#-commit-message-guidelines
- https://gist.github.com/qoomon/5dfcdf8eec66a051ecd85625518cfd13

## Reuse Code in LabVIEW
- https://learn.ni.com/pages/seta
- https://learn.ni.com/learn/learning-path/implementing-reuse-strategies
- https://learn.ni.com/learn/learning-path/implementing-a-test-strategy-in-labview
- https://learn.ni.com/learn/learning-path/source-code-control
- https://learn.ni.com/learn/learning-path/continuous-integration
- https://learn.ni.com/learn/learning-path/requirements
- https://learn.ni.com/learn/learning-path/project-management

## LabVIEW
- https://www.youtube.com/@TomsLabVIEWAdventure

## Object Oriented Programming in LabVIEW
- https://youtube.com/playlist?list=PLmF-6jvwRvVNVPfGxGPMsf3cZafT83oH8&si=R42QMkmSuOCQfr5-

## The Actor Framework in LabVIEW
- https://youtube.com/playlist?list=PLmF-6jvwRvVNFzBjzh4bQDjFbv6lShcth&si=-p_imQLMUj1k1E8p


This README.md document can be found and edited at the following location: `key-es/.github/profile/README.md`
