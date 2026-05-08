# AI 辅助建模工作流

用 Codex Skills 驱动 Blender MCP，为 CS:CZ Source 项目进行参考驱动、分步验证的 3D 资产制作。

## 技能（Skills）

| 技能 | 作用 |
|---|---|
| `blender-superskill` | Blender 建模方法论——参考优先、分步构建、视口检查、失败修复 |
| `cs-czs-project` | 本项目专属知识——目录结构、资产管线、模型对照链、标准模型 |

AI 激活上述技能后，会自动：
- 先查阅对应类型的**标准模型**（`models/*/standard/`），搞清面数/比例/结构标杆
- 三层对照：源文件(.smd/.qc) → 编译产物(game_res) → 引擎源码(game_src)
- 分步建模，每步对照参考图检查，不合格就迭代

