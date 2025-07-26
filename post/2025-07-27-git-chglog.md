---
show_subscribe: false

title: git-chglog 自动生产 CHANGES
tags:
    - git
---

## [git-chglog](https://github.com/git-chglog/git-chglog) 自动生成 changes log

### Mac 上安装使用

[Homebrew](https://brew.sh/) (for macOS users)
```shell
brew tap git-chglog/git-chglog
brew install git-chglog
```

### 使用
执行命令后， 会自动生成模版和配置文件
```shell
git-chglog --init
```

Help
```shell
$ git-chglog --help

USAGE:
  git-chglog [options] <tag query>

    There are the following specification methods for <tag query>.

    1. <old>..<new> - Commit contained in <old> tags from <new>.
    2. <name>..     - Commit from the <name> to the latest tag.
    3. ..<name>     - Commit from the oldest tag to <name>.
    4. <name>       - Commit contained in <name>.

OPTIONS:
  --init                      generate the git-chglog configuration file in interactive (default: false)
  --path value                Filter commits by path(s). Can use multiple times.
  --config value, -c value    specifies a different configuration file to pick up (default: ".chglog/config.yml")
  --template value, -t value  specifies a template file to pick up. If not specified, use the one in config
  --repository-url value      specifies git repo URL. If not specified, use 'repository_url' in config
  --output value, -o value    output path and filename for the changelogs. If not specified, output to stdout
  --next-tag value            treat unreleased commits as specified tags (EXPERIMENTAL)
  --silent                    disable stdout output (default: false)
  --no-color                  disable color output (default: false) [$NO_COLOR]
  --no-emoji                  disable emoji output (default: false) [$NO_EMOJI]
  --no-case                   disable case sensitive filters (default: false)
  --tag-filter-pattern value  Regular expression of tag filter. Is specified, only matched tags will be picked
  --jira-url value            Jira URL [$JIRA_URL]
  --jira-username value       Jira username [$JIRA_USERNAME]
  --jira-token value          Jira token [$JIRA_TOKEN]
  --sort value                Specify how to sort tags; currently supports "date" or by "semver" (default: date)
  --help, -h                  show help (default: false)
  --version, -v               print the version (default: false)

EXAMPLE:

  $ git-chglog

    If <tag query> is not specified, it corresponds to all tags.
    This is the simplest example.

  $ git-chglog 1.0.0..2.0.0

    The above is a command to generate CHANGELOG including commit of 1.0.0 to 2.0.0.

  $ git-chglog 1.0.0

    The above is a command to generate CHANGELOG including commit of only 1.0.0.

  $ git-chglog $(git describe --tags $(git rev-list --tags --max-count=1))

    The above is a command to generate CHANGELOG with the commit included in the latest tag.

  $ git-chglog --output CHANGELOG.md

    The above is a command to output to CHANGELOG.md instead of standard output.

  $ git-chglog --config custom/dir/config.yml

    The above is a command that uses a configuration file placed other than ".chglog/config.yml".

  $ git-chglog --path path/to/my/component --output CHANGELOG.component.md

    Filter commits by specific paths or files in git and output to a component specific changelog.
```
