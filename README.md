# gh-vulns

This displays all vulnerabilities in your own repositories.

![image](https://user-images.githubusercontent.com/10758173/120782092-9f99f280-c564-11eb-9443-90d8f2851adb.png)

## Requirements 

- [gh](https://github.com/cli/cli)
- [jq](https://github.com/stedolan/jq)
- [Zsh](https://zsh.sourceforge.io/)

## Installation

zinit

```zsh
zinit ice lucid as'program'
zinit light hexium310/gh-vulns
```

Or install this on your `$PATH`.

## Usage

You can pass a GitHub username that have repositories you want to get vulnerabilities or set it to `$GH_VULNS_USERNAME`.
When a username isn't passed and `$GH_VULNS_USERNAME` isn't set, the one got using GitHub API is used.

```
gh-vulns hexium310

# Using $GH_VULNS_USERNAME or GitHub API
gh-vulns
```

Besides, you can create a alias for `gh`.


```
gh alias set --shell vulns 'gh-vulns'
```
