# openSUSE
### 1. **安装软件包**
```bash
zypper install <package-name>
```
- 安装指定的软件包。

### 2. **卸载软件包**
```bash
zypper remove <package-name>
```
- 卸载指定的软件包。

### 3. **更新软件包**
```bash
zypper update <package-name>
```
- 更新指定的软件包到最新版本。

### 4. **更新所有软件包**
```bash
zypper update
```
- 更新系统中所有安装的软件包。

### 5. **升级系统**
```bash
zypper dup
```
- 升级系统，尤其是进行发行版升级时使用。

### 6. **查找软件包**
```bash
zypper search <package-name>
```
- 搜索可用的软件包。

### 7. **显示软件包信息**
```bash
zypper info <package-name>
```
- 显示指定软件包的详细信息（如版本、依赖关系等）。

### 8. **列出已安装的软件包**
```bash
zypper list-updates
```
- 列出所有可以更新的软件包。

### 9. **添加软件仓库**
```bash
zypper addrepo <url> <repo-name>
```
- 添加新的软件仓库。

### 10. **列出已添加的仓库**
```bash
zypper repos
```
- 显示所有已添加的软件仓库。

### 11. **删除软件仓库**
```bash
zypper removerepo <repo-name>
```
- 删除指定的软件仓库。

### 12. **刷新软件仓库**
```bash
zypper refresh
```
- 刷新所有已配置的仓库，获取最新的软件包信息。

### 13. **清理缓存**
```bash
zypper clean
```
- 清理 `zypper` 的缓存，以释放磁盘空间。

### 14. **解决依赖问题**
```bash
zypper verify
```
- 检查并修复系统中的依赖问题。

### 15. **显示安装软件包的依赖关系**
```bash
zypper info --requires <package-name>
```
- 显示指定软件包的依赖关系。

### 16. **列出所有软件包的版本信息**
```bash
zypper versions
```
- 显示所有已安装的软件包的版本信息。

### 17. **安装指定版本的软件包**
```bash
zypper install <package-name>=<version>
```
- 安装特定版本的软件包。

### 18. **锁定软件包版本**
```bash
zypper addlock <package-name>
```
- 锁定某个软件包的当前版本，避免其被更新。

### 19. **解锁软件包**
```bash
zypper removerlock <package-name>
```
- 解锁某个已锁定的软件包，允许其进行更新。

### 20. **查询软件包的提供者**
```bash
zypper what-provides <file>
```
- 查询提供特定文件或程序的包。

### 21. **查看软件包的变更日志**
```bash
zypper changelog <package-name>
```
- 查看指定软件包的变更日志。

### 22. **显示某个软件包的安装文件**
```bash
zypper info --provides <package-name>
```
- 显示指定软件包提供的文件或功能。

### 23. **检查并修复系统**
```bash
zypper dup --no-verify
```
- 在系统升级过程中，跳过验证步骤（适用于出现安装问题时）。

### 24. **安装所有可用的更新（包括未安装的软件包）**
```bash
zypper update --all
```
- 更新系统，安装所有可用的更新，包括那些尚未安装的软件包。

### 25. **导入 GPG 密钥**
```bash
zypper import-gpg <key-file>
```
要列出所有已安装的软件包，可以使用以下命令：

```bash
zypper se --installed-only
```

或简化为：

```bash
zypper search --installed-only
```

这会列出系统上所有已安装的软件包。

如果你希望查看更详细的包信息（例如版本号、架构等），可以使用：

```bash
zypper info --installed-only
```

这个命令会列出每个已安装包的详细信息。如果只是想查看软件包名称和版本，可以使用：

```bash
rpm -qa
```

`rpm -qa` 是 `zypper` 的底层包管理工具，可以列出所有已安装的 RPM 包。
- 导入 GPG 密钥文件，用于验证仓库的包。

---

这些是 `zypper` 常用的命令。如果你想进一步了解某个命令的用法，可以通过以下命令查看帮助：

```bash
zypper --help
```

这个命令将列出所有 `zypper` 命令的选项和用法。
