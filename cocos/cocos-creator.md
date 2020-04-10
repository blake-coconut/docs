# Cocos Creator

## 设置

### 设置VS Code为脚本编辑器

打开**Cocos Creator**进入**偏好设置**选择**数据编辑**，在**外部脚本编辑器**中选择**VS Code**，
这样在**Cocos Creator**中双击脚本文件时，会自动跳转至**VS Code**中进行编辑。

---

## 项目结构

*注意：Cocos Creator 使用特定结构的文件夹来作为合法项目标识，而不是使用工程文件。*

```markdown
.
├── assets              # 资源文件夹
├── library             # 资源库（不进入版本控制）
├── local               # 本地设置（不进入版本控制）
├── packages            # 扩展插件文件夹
├── settings            # 项目设置
├── temp                # 临时文件夹
├── build               # 构建目标（不进入版本控制）
└── project.json
```

[详情文档](https://docs.cocos.com/creator/1.10/manual/zh/getting-started/project-structure.html)
