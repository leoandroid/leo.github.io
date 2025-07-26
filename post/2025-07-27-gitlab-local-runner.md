---
show_subscribe: false

title: 'Gitlab 部署 runner'
date: 2025-07-27
excerpt: 'Gitlab 本地部署 Runner 运行 CI/CD'
tags:
  - Gitlab
  - Devops
---

[[_TOC_]]

## GitLab Runner 配置

**工作目录位置**
`${HOME}/builds/<unique-id>/<project-path>`

**注册命令示例**：

```shell
sudo gitlab-runner register
Runtime platform      arch=arm64 os=darwin pid=81548 revision=2b813ade version=18.1.1

# 按提示输入以下信息：
GitLab 实例 URL： gitlab 仓库 URL
注册令牌：         gitlab 令牌
Runner 描述：     关于  runner 的简单描述
标签：            tag 在写 CI/CD 脚本时需要使用
执行器类型：       shell, 因为我们是在  mac 上部署， 所以这里选 shell
```

**注册命令**：
```shell
➜  ~ sudo gitlab-runner register
Password:
Runtime platform                                    arch=arm64 os=darwin pid=81548 revision=2b813ade version=18.1.1
Running in system-mode.

Created missing unique system ID                    system_id=s_5944e08b6352
Enter the GitLab instance URL (for example, https://gitlab.com/):
https://gitlab.com/
Enter the registration token:
token
Enter a description for the runner:
[MacBook.local]: 描述这是一个什么 runner
Enter tags for the runner (comma-separated):
runner tag
Enter optional maintenance note for the runner:
描述
WARNING: Support for registration tokens and runner parameters in the 'register' command has been deprecated in GitLab Runner 15.6 and will be replaced with support for authentication tokens. For more information, see https://docs.gitlab.com/ci/runners/new_creation_workflow/
Registering runner... succeeded                     correlation_id=1P0fJ8OCUX5 runner=JHLoeVy-
Enter an executor: shell, ssh, docker, docker+machine, docker-autoscaler, custom, parallels, virtualbox, docker-windows, kubernetes, instance:
shell
Runner registered successfully. Feel free to start it, but if it's running already the config should be automatically reloaded!

Configuration (with the authentication token) was saved in "/etc/gitlab-runner/config.toml"
```

## 本地 Runner 管理

**常用操作命令**

| 操作 | 命令 | 说明 |
|------|------|------|
| 启动服务 | `brew services start gitlab-runner` | 后台运行 Runner |
| 验证状态 | `sudo gitlab-runner verify` | 检查 Runner 活性 |
| 停止服务 | `brew services stop gitlab-runner` | 停止后台运行 |
| 查看日志 | `tail -f /usr/local/var/log/gitlab-runner.log` | 监控运行状态 |
