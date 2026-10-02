# Autonomous Game Studio

使用 Godot 开发游戏，使用 Blender 制作美术资源。

## 目录

```text
game/          Godot 工程及游戏运行时资源
art/blender/   Blender 源文件（.blend）
docs/          游戏设计、开发记录和资源规范
build/         本地构建产物（不提交）
```

当前仅建立仓库骨架，尚未创建 Godot 工程或确定工具版本。

## 开始开发

1. 确定游戏类型、目标平台及 Godot、Blender 版本，并在此记录。
2. 在 Godot 中创建工程，将工程路径设为本仓库的 `game/`。
3. 将 Blender 源文件保存到 `art/blender/`；供游戏使用的导出资源放入 `game/assets/`。
4. 将玩法设计、操作方式和开发约定记录到 `docs/`。

## 资源与版本管理

- 提交 Godot 工程、脚本、场景、原始资源及 `.uid`、`.import` 元数据文件；忽略生成的 `.godot/` 和 `.import/` 缓存目录。
- 提交 `.blend` 源文件；忽略 `.blend1` 等备份文件。
- 3D 模型可从 Blender 导出为 `.glb` 后放入 Godot 工程；具体导出规范随项目需求确定。
- 构建产物统一放入根目录的 `build/`。
- 大型二进制资源增加后，按需要配置 Git LFS。
