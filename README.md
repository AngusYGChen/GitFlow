# GitFlow
Git Flow Template

## 核心分支

### 1. main branch

- 版本号规则：主版本号.次版本号.修订号
    - 主版本号：主要功能变化和重大更新
    - 次版本号：功能的改进和更新
    - 修订号：bug 和补丁修复
- 更新限制：只接受来自 `hotfix branch` 和 `release branch` 的合并请求

### 2. develop branch

- 与 `main branch` 分离，用于开发和测试


## 辅助分支

### 1. hotfix branch

- 基于 `main branch`，用于线上版本的热修复
- 命名规则：`hotfix-#{issueid}-{desc}`
- 完成后需要同时合并到 `main branch` 和 `develop branch`
- 需要更新修订号

### 2. release branch

- 基于 `develop branch`，用于测试和验证要发布的版本
- 需要将每一个 commit cherry-pick 到 `develop branch`
- 完成后需要合并到 `main branch`
- 根据需要更新版本号

### 3. feature branch

- 基于 `develop branch`，用于开发和管理某个具体的功能
- 命名规则：`feature-{featureName}`
- 完成后需要合并到 `develop branch`









