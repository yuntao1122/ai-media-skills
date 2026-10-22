# AI Media Skills

一套开源的 AI 媒体创作技能包。把"搜集、筛选、做图片、做视频"四条高频 AI 工作流，打包成标准的 Agent Skills（`SKILL.md`），任何支持该标准的 AI agent 装上就能直接用。

## Skills

| Skill | 干什么 | 什么时候用 |
|---|---|---|
| `hunter` | 全网素材搜集：多渠道检索、来源分级、输出带摘要的素材清单 | 要调研、找资料、攒素材时 |
| `curator` | 素材筛选：去重、四维打分、分级精选 | 素材太多、要挑出能用的时 |
| `imager` | AI 图片工作流：prompt 模板、评审迭代、多尺寸适配 | 要配图、海报、封面、插画时 |
| `director` | AI 视频工作流：分镜脚本、片段生成、组装成片 | 要做短视频、解说、混剪时 |

四个 skill 可以串起来用：一个选题从 `hunter` 搜集 → `curator` 筛选 → `imager` 配图 → `director` 成片。

## 快速开始

1. 把 `skills/` 下对应目录放进你的 agent 的 skills 目录（或按你所用平台的 skill 安装方式加载）。
2. 每个 skill 的用法都在各自的 `SKILL.md` 里：触发条件、输入、完整工作流、输出模板。
3. 直接对 agent 说"用 hunter 帮我搜集 XX 素材"即可。

## 目录结构

```
ai-media-skills/
├── README.md
├── LICENSE
└── skills/
    ├── hunter/SKILL.md      # 搜集
    ├── curator/SKILL.md     # 筛选
    ├── imager/SKILL.md      # 图片
    └── director/SKILL.md    # 视频
```

## 路线图

- [ ] 给每个 skill 配可运行的辅助脚本（去重、评分表生成等）
- [ ] 增加 `podcaster`（播客/音频工作流）
- [ ] 增加英文版 SKILL.md
- [ ] 示例：用四个 skill 完整做一期视频的全流程演示

## 参与贡献

欢迎提 Issue 和 PR。新增 skill 请按现有格式写 `SKILL.md`：触发条件、输入、工作流、输出模板、注意事项五部分。

## License

MIT，见 [LICENSE](LICENSE)。
