# Mia 周期化训练计划

一个用于 Codex 和 ChatGPT 的周期化训练计划 skill。

它以 Andy Galpin 课程中的“大目标 → 限制因素 → 训练分块 → 微周期”规划思路为基础，并针对 Mia 的核心人群加入日程约束、普通成年训练者的安全边界、忙碌周最小方案和反馈驱动的调整规则。

## 能做什么

- 从零制定 4–16 周增肌、力量、体能或减脂配套训练计划
- 把年度目标拆成中周期、训练块和每周安排
- 审查现有计划的目标、负荷、恢复和进阶逻辑
- 根据完成率、RPE/RIR、疲劳、疼痛与表现迭代下一周期
- 区分进阶、保持、回调和停止训练的条件

## 安装

在 Codex CLI 中添加这个 GitHub marketplace：

```bash
codex plugin marketplace add miaxie88/mia-periodized-training-planner
```

随后：

1. 重启 ChatGPT 桌面应用或 Codex。
2. 打开 Plugins Directory。
3. 选择 `Mia Skills`。
4. 安装 `Mia 周期化训练计划`。
5. 开启一个新对话。

安装后可以直接输入：

```text
$mia-periodized-training-planner
```

示例：

```text
使用 $mia-periodized-training-planner，根据我每周可训练 3 天、每次 45 分钟的情况，制定一个 12 周全身力量与增肌计划。
```

## 仓库结构

```text
.agents/plugins/marketplace.json
plugins/mia-periodized-training-planner/
├── .codex-plugin/plugin.json
└── skills/mia-periodized-training-planner/
    ├── SKILL.md
    ├── agents/openai.yaml
    └── references/
        ├── methodology.md
        ├── plan-template.md
        └── source-map.md
```

## 方法论

```text
真实日程
→ 一个主目标
→ 1–3 个限制因素
→ 训练块顺序与时长
→ 周计划与单次课表
→ 进阶、保持、回调或停止
```

周期化是有意图的变化，不是随机更换动作。计划先确定目标与限制因素，再选择频率、动作、强度、训练量与休息。

## 来源与独立性说明

本项目参考了 Andy Galpin 关于 periodization 与 program design 的公开教育内容，并进行了独立提炼与适用场景改写。它不是 Andy Galpin 的官方产品，也不代表其本人或所属机构的背书。

仓库不包含原始视频、完整字幕或长篇逐字转录。`source-map.md` 仅记录方法论对应的时间段、术语校正和二次设计边界。

## 健康与安全声明

本项目只提供一般训练规划参考，不提供医疗诊断、伤病康复、术后康复、心脏康复、药物或饮食处方。

如有急性伤病、持续或加重的疼痛、胸痛、晕厥、异常呼吸困难或新发神经症状，请停止训练并先寻求专业评估。孕期、产后、儿童青少年、高龄体弱者、慢性病患者和正在用药者，需要结合医生或合格专业人士的个体建议。

## 版本

- `0.1.0`：首次公开版本

## License

暂未授予开源许可。若希望复制、修改或再分发，请先联系仓库作者。
