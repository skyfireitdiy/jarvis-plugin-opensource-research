# 开源项目研究插件（opensource-research）
> Jarvis 外部插件：**开源项目研究**。
> 系统性研究开源项目——提供开源软件研究的九阶段方法论，生成深度研究报告。

## 功能

- **九阶段研究方法论**：背景研究 → 问题与解决方案 → 关键技术 → 架构设计 → 优缺点 → 竞品分析 → 演进方向 → 跟进策略 → 总结报告。
- 每个阶段提供结构化研究框架与输出模板，引导 Agent 系统化完成开源项目调研。
- 纯规则集插件，无额外依赖，安装即可生效。

## 安装

### 从插件市场安装（推荐）
在 Jarvis 插件管理面板的「市场」页签搜索 `opensource-research`，一键安装。

### 命令行安装
```bash
# 从源码仓库安装
jarvis --install-plugin https://github.com/skyfireitdiy/jarvis-plugin-opensource-research
# 或从本地目录安装
jarvis --install-plugin /path/to/opensource-research
```
安装后重启 Jarvis 使插件注册生效：
```bash
jarvis --list-plugins   # 确认 opensource-research 插件已注册
```

### 卸载
```bash
jarvis --uninstall-plugin opensource-research
```

> 注：opensource-research 已从 Jarvis 核心内置插件迁移为独立第三方插件（见 [Issue #273](https://github.com/skyfireitdiy/Jarvis/issues/273)）。旧版本内置插件用户升级后需从市场重新安装。

## 目录结构
```text
opensource-research/
├── config.yaml          # 插件配置：logo、rules_load_dirs
├── frontend/
│   └── icon.svg         # 插件图标
└── rules/
    ├── opensource_research.md          # 九阶段方法论总纲
    └── opensource_research/            # 各阶段详细规则
        ├── 01_background_research.md   # 背景研究
        ├── 02_problem_solution.md      # 问题与解决方案
        ├── 03_key_technologies.md      # 关键技术
        ├── 04_architecture_design.md   # 架构设计
        ├── 05_pros_cons.md             # 优缺点
        ├── 06_competitor_analysis.md   # 竞品分析
        ├── 07_evolution_direction.md   # 演进方向
        ├── 08_followup_strategy.md     # 跟进策略
        └── 09_summary_report.md        # 总结报告
```

## 九阶段方法论
1. **背景研究**：项目定位、历史沿革、社区生态。
2. **问题与解决方案**：解决的核心问题、方案对比。
3. **关键技术**：核心技术栈、实现要点。
4. **架构设计**：整体架构、模块划分、数据流。
5. **优缺点**：优势与局限分析。
6. **竞品分析**：同类项目横向对比。
7. **演进方向**：Roadmap、社区趋势。
8. **跟进策略**：如何跟进、参与贡献。
9. **总结报告**：综合输出深度研究报告。

## License
MIT
