# Hi there 👋

<!--
Comments
🧙 Remember, you can do mighty things with the power of [Markdown](https://docs.github.com/github/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax)
-->

The key-es GitHub organisation is for internal sharing of reuse code.

# Source Control

## Setup

Create a new repository on GitHub

`git clone git@github.com:user-name/repo-name.git`

Create `dev` branch in GitHub

`git pull`

`git switch dev`

## Branches

|Branch Name|Description|
|-----------|-----------|
|`main`|Release branch|
|`dev`|Development branch|
|`[issue-id]`|Development on a particular issue|

## Conventional Commits

https://www.conventionalcommits.org/en/v1.0.0
https://github.com/angular/angular/blob/22b96b9/CONTRIBUTING.md#-commit-message-guidelines
https://gist.github.com/qoomon/5dfcdf8eec66a051ecd85625518cfd13

## Issues


## Releases

`git add .`

`git commit -m 'Release 1.0.0'`

`git tag -a 1.0.0 -m 'Release 1.0.0 - first release'`

`git push origin main --tags`


# Versioning

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



# Useful Resources

https://semver.org/

https://learn.ni.com/pages/seta
https://learn.ni.com/learn/learning-path/implementing-reuse-strategies
https://learn.ni.com/learn/learning-path/implementing-a-test-strategy-in-labview
https://learn.ni.com/learn/learning-path/source-code-control
https://learn.ni.com/learn/learning-path/continuous-integration
https://learn.ni.com/learn/learning-path/requirements
https://learn.ni.com/learn/learning-path/project-management

https://www.youtube.com/@TomsLabVIEWAdventure
OOP
https://youtube.com/playlist?list=PLmF-6jvwRvVNVPfGxGPMsf3cZafT83oH8&si=R42QMkmSuOCQfr5-
Actor Framework
https://youtube.com/playlist?list=PLmF-6jvwRvVNFzBjzh4bQDjFbv6lShcth&si=-p_imQLMUj1k1E8p
