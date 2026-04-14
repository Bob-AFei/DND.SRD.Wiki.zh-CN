# DND.SRD.Wiki 与 DND5e_chm 结构对应关系

## 零、翻译资源优先级

本项目翻译时遵循以下资源优先级：

| 优先级 | 资源 | 定位 | 说明 |
|---------|---------|---------|--------|
| **1（最高）** | `SRD_CC_v5.2.1.md` | **最权威英文来源** | Wizards of the Coast 官方发布，所有翻译文本最终以此为准 |
| **2** | `DND.SRD.Wiki/` | **格式与结构参考** | Markdown 格式、文件结构和目录组织的主要参考 |
| **3** | `DND5e_chm/` | **中文术语参考** | 中文官方译名、术语一致性的主要参考源 |

> **重要说明：** 当 DND.SRD.Wiki 内容与 SRD_CC_v5.2.1.md 存在出入时，一律以 SRD 官方文档为准。翻译完成后必须对照 SRD 官方文档进行最终校对。

---

## 一、顶级目录对应关系

### 完全对应的内容
```
DND.SRD.Wiki/Classes/          ↔ DND5e_chm/玩家手册/职业/
DND.SRD.Wiki/Races/            ↔ DND5e_chm/玩家手册/种族/
DND.SRD.Wiki/Equipment/        ↔ DND5e_chm/玩家手册/装备/
DND.SRD.Wiki/Spells/           ↔ DND5e_chm/玩家手册/魔法/
DND.SRD.Wiki/Gameplay/         ↔ DND5e_chm/玩家手册/进行游戏/
DND.SRD.Wiki/Gamemastering/    ↔ DND5e_chm/城主指南/
DND.SRD.Wiki/Characterizations/↔ DND5e_chm/玩家手册/个性与背景/
```

### 部分对应的内容
```
DND.SRD.Wiki/Monsters/         ↔ DND5e_chm/怪物图鉴/ (+ 类人生物等子目录)
DND.SRD.Wiki/Treasure/         ↔ DND5e_chm/怪物图鉴/ (战利品部分) + 玩家手册/装备/
```

---

## 二、详细文件对应清单

### 1. 职业（Classes）

**文件数量：** 12 个职业

**翻译状态：** ✅ **已完成**

| 英文原版 | 中文版本 | 职业特色 |
|---------|---------|---------|
| Barbarian.md | 野蛮人.md | 狂暴、生存能力 |
| Bard.md | 吟游诗人.md | 演艺、魅惑、支援 |
| Cleric.md | 牧师.md | 治疗、牧师法术 |
| Druid.md | 德鲁伊.md | 自然、野性塑形 |
| Fighter.md | 战士.md | 攻击多样、防御 |
| Monk.md | 武僧.md | 格斗、气功、速度 |
| Paladin.md | 圣武士.md | 圣魔、制裁一击 |
| Ranger.md | 游侠.md | 追踪、生存、远程 |
| Rogue.md | 游荡者.md | 潜行、偷袭、盗窃 |
| Sorcerer.md | 术士.md | 血统法术、灵活 |
| Warlock.md | 邪术师.md | 契约、邪术、诡计 |
| Wizard.md | 法师.md | 学术法术、知识 |

**职业文件结构示例（Fighter.md）：**
```
# Fighter
  ### Class Features
    #### Hit Points
    #### Proficiencies
    #### Equipment
  ### Table: The Fighter
  ### Fighting Style
  ### Second Wind
  ### Action Surge
  ### Martial Archetype
  ### Extra Attack
  ### Indomitable
  [更多等级相关特性...]
```

**文件大小范围：** 100-200 行

---

### 2. 法术（Spells）

**文件数量：** 322 个法术

**翻译状态：** 🟡 **部分完成（戏法 24 个）**

**组织方式：**
- 按法术学派和环阶组织
- 主要包括：戏法（0环）到9环法术

**已翻译戏法列表（24个）：**
- 酸液飞溅 Acid Splash（咒法）
- 冻死之触 Chill Touch（死灵）
- 舞光术 Dancing Lights（塑能）
- 德鲁伊伎俩 Druidcraft（变化）
- 魔能爆 Eldritch Blast（塑能）
- 火焰箭 Fire Bolt（塑能）
- 指导术 Guidance（预言）
- 光亮术 Light（塑能）
- 法师之手 Mage Hand（咒法）
- 修复术 Mending（变化）
- 传讯术 Message（变化）
- 次级幻影 Minor Illusion（幻术）
- 毒气喷溅 Poison Spray（咒法）
- 魔法伎俩 Prestidigitation（变化）
- 产生火焰 Produce Flame（咒法）
- 冻霜射线 Ray of Frost（塑能）
- 抗性术 Resistance（防护）
- 圣火术 Sacred Flame（塑能）
- 橡棍术 Shillelagh（变化）
- 电击掌 Shocking Grasp（塑能）
- 救命术 Spare the Dying（死灵）
- 奇术 Thaumaturgy（变化）
- 克敌机先 True Strike（预言）
- 恶毒嘲笑 Vicious Mockery（附魔）

**法术学派对应：**
```
Abjuration     ↔ 防护
Conjuration    ↔ 咒法
Divination     ↔ 预言
Enchantment    ↔ 附魔
Evocation      ↔ 塑能
Illusion       ↔ 幻术
Necromancy     ↔ 死灵
Transmutation  ↔ 变化
```

**法术文件结构示例（Acid Splash.md）：**
```
### Acid Splash

*Conjuration cantrip*

**Casting Time:** 1 action
**Range:** 60 feet
**Components:** V, S
**Duration:** Instantaneous

[描述文本]

This spell's damage increases by 1d6 when you reach 5th level (2d6), 
11th level (3d6), and 17th level (4d6).
```

**文件大小范围：** 10-50 行（多数为 15-30 行）

**中文版本存储方式：**
```
DND5e_chm/玩家手册/魔法/法术详述/
├── 戏法.html         (所有0环法术)
├── 1环.html          (所有1环法术)
├── 2环.html
├── ...
├── 9环.html
└── 法术列表/         (按职业分类)
    ├── 牧师法术.html
    ├── 法师法术.html
    └── ...
```

---

### 3. 怪物（Monsters）

**文件数量：** 319 个怪物

**怪物分类对应（按中文版本分类）：**

| 英文原版分类 | 中文分类 | 数量 | 文件数 |
|-------------|---------|------|--------|
| Beast | 野兽 | 多种动物 | 55 |
| Dragon | 龙类 | 各色龙类 | 50 |
| Monstrosity | 怪兽 | 异形生物 | 53 |
| Humanoid (NPC) | 类人生物/非玩家角色 | 商人、卫兵等 | 37 |
| Fiend | 邪魔 | 恶魔、魔鬼 | 37 |
| Creature Template | 模板生物 | 变种模板 | 20 |
| Undead | 不死生物 | 丧尸、幽灵 | 19 |
| Construct | 构装生物 | 魔法造物 | 19 |
| Elemental | 元素生物 | 各类元素体 | 25 |
| 其他 | 精类、巨人、泥怪等 | 多种 | 48 |

**怪物文件结构示例（Aboleth.md）：**
```
## Aboleth

*Large aberration, lawful evil*

**Armor Class** 17 (natural armor)
**Hit Points** 135 (18d10+36)
**Speed** 10 ft., swim 40 ft.

| STR | DEX | CON | INT | WIS | CHA |
|-----|-----|-----|-----|-----|-----|
| 21 (+5) | 9 (-1) | 15 (+2) | 18 (+4) | 15 (+2) | 18 (+4) |

**Saving Throws** Con +6, Int +8, Wis +6
**Skills** History +12, Perception +10
**Senses** darkvision 120 ft., passive Perception 20
**Languages** Deep Speech, telepathy 120 ft.
**Challenge** 10 (5,900 XP)

***特殊能力 1***. 描述...
***特殊能力 2***. 描述...

###### Actions
***Multiattack***. ...
***Tentacle***. *Melee Weapon Attack:* +9 to hit...
***Tail***. ...

###### Legendary Actions
...
```

**文件大小范围：** 30-100 行

---

### 4. 装备（Equipment）

**文件数量：** 9 个主要文件

**文件对应：**
```
Armor.md              ↔ 护甲与盾牌.html
Weapons.md            ↔ 武器.html
Coinage.md            ↔ 财富.html
Expenses.md           ↔ 其他开支.html
Gear.md               ↔ 冒险用品.html
Tools.md              ↔ 工具.html
Trade Goods.md        ↔ 商品.html
Transportation.md     ↔ 坐骑与载具.html
Selling Treasure.md   ↔ [部分内容在宝物部分]
```

**装备文件结构示例（Weapons.md）：**
```
# Weapons

[介绍段落]

## Weapon Proficiency
[描述]

## Weapon Properties
- ***Ammunition***. [描述]
- ***Finesse***. [描述]
- ***Heavy***. [描述]
...

### Melee Weapons
| Name | Cost | Damage | Weight | Properties |
| ... | ... | ... | ... | ... |

### Ranged Weapons
| Name | Cost | Damage | Weight | Properties |
| ... | ... | ... | ... | ... |
```

**文件大小范围：** 50-150 行

---

### 5. 种族（Races）

**文件数量：** 10 个主要种族

**翻译状态：** ✅ **已完成**

| 英文原版 | 中文版本 | 说明 |
|---------|---------|------|
| *(种族特征总述)* | # 种族特征.md | 种族通用特征说明 |
| Dragonborn.md | 龙裔.md | 龙息武器、龙裔抗性 |
| Dwarf.md | 矮人.md | 矮人强韧、战斗训练 |
| Elf.md | 精灵.md | 精灵感知、恍惚冥想 |
| Gnome.md | 侏儒.md | 侏儒狡黠、先天法术 |
| Half-Elf.md | 半精灵.md | 技能多样、黑暗视觉 |
| Half-Orc.md | 半兽人.md | 坚不可摧、残暴攻击 |
| Halfling.md | 半身人.md | 幸运、勇敢、半身人灵巧 |
| Human.md | 人类.md | 属性全面提升 |
| Tiefling.md | 提夫林.md | 地狱遗产、先天法术 |

**文件大小范围：** 50-150 行

---

### 6. 背景和特征（Characterizations）

**文件数量：** 7 个文件

**翻译状态：** ✅ **已完成**

| 英文 | 中文 | 翻译状态 |
|-----|-----|---------|
| Alignment.md | 阵营.md | ✅ 已完成 |
| Backgrounds.md | 背景.md | ✅ 已完成 |
| Feats.md | 专长.md | ✅ 已完成 |
| Inspiration.md | 灵感.md | ✅ 已完成 |
| Languages.md | 语言.md | ✅ 已完成 |
| Multiclassing.md | 兼职.md | ✅ 已完成 |
| Beyond 1st Level.md | 超越1级.md | ✅ 已完成 |

---

### 7. 游戏规则（Gameplay）

**文件数量：** 3 个文件

**翻译状态：** ✅ **已完成**

| 英文 | 中文 |
|-----|-----|
| Abilities.md | 属性值.md |
| Adventuring.md | 冒险.md |
| Combat.md | 战斗.md |

---

### 8. 城主指南（Gamemastering）

**文件数量：** 8 个文件

| 英文 | 中文 |
|-----|-----|
| Conditions.md | 状态 |
| Diseases.md | 疾病 |
| Madness.md | 疯狂 |
| Objects.md | 物体 |
| Pantheons.md | 神系 |
| Planes.md | 位面 |
| Poisons.md | 毒物 |
| Traps.md | 陷阱 |

---

## 三、内容转换指南

### Markdown 到 HTML 转换建议

**English Markdown 特征：**
```markdown
# 一级标题 (h1)
### 三级标题 (h3) - 最常用
#### 四级标题 (h4)

**粗体**
*斜体*
***加粗斜体***

| Table | Format |
|-------|--------|
| Data  | Data   |

- 列表项
  - 嵌套项

> 引用
```

**中文 HTML 对应样式：**
- 标题用 `<h1>`, `<h3>`, `<h4>` 标签
- 专业术语保持中英对照
- 表格使用 `<table>` 标签
- 保留格式化属性（加粗、斜体）

---

## 四、关键注意事项

### 1. 术语一致性
- **术语优先级**：参考 `DND5e_术语对照表.csv`
- **上下文差异**：同一词在不同上下文可能有不同翻译
  - 例如：Range 在装备中是"射程"，在法术中是"施法距离"

### 2. 数据结构
- 属性表必须保持一致格式
- 怪物属性值表（STR/DEX/CON/INT/WIS/CHA）必须完整
- 法术成分（V/S/M）的格式统一

### 3. 特殊格式
- ***粗体斜体*** 用于特殊能力名称
- **粗体** 用于关键术语
- 数据表使用一致的列格式

### 4. 翻译规范补充
- 列表序号（如 a, b, c）保持原样，不翻译为甲、乙、丙

### 5. 翻译审查清单
- [ ] 职业特性名称是否一致
- [ ] 法术学派翻译是否统一
- [ ] 怪物类型分类是否对应
- [ ] 装备属性名称是否规范
- [ ] 数值格式是否一致（如 1d6 vs 1d6）

### 6. 翻译后对比检查

翻译完成后，必须自动对比 DND5e_chm 目录中的中文参考资料，进行完整性检查和术语校准：

**检查要点：**
- [ ] 专业术语是否与 DND5e_chm 中文参考一致
- [ ] 特性名称、技能名称、法术名称是否采用标准译法
- [ ] 属性描述、数值、表格内容是否完整无遗漏
- [ ] 关键信息（特性效果、条件限制、持续时间等）是否完整
- [ ] 规则性描述是否准确传达游戏机制含义

**对比优先级：**
- 内容准确性：SRD_CC_v5.2.1.md > DND5e_chm
- 术语表达：DND5e_chm > 自行翻译
- 信息完整性：两者结合，确保 SRD 范围内信息完整
- 格式规范：DND.SRD.Wiki 的 Markdown 格式为准

**参考路径速查：**

| 翻译类别 | DND5e_chm 参考路径 | 说明 |
|----------|-------------------|------|
| 职业 | `玩家手册/职业/` | 12个职业完整资料 |
| 种族 | `玩家手册/种族/` | 10个基础种族 |
| 法术 | `玩家手册/魔法/法术详述/` | 按环阶分文件（戏法到9环） |
| 装备 | `玩家手册/装备/` | 武器、护甲、冒险用品等 |
| 怪物 | `怪物图鉴/` | 按生物类型分子目录 |
| 游戏规则 | `玩家手册/进行游戏/` + `属性值应用/` + `战斗/` | 基础规则 |
| 背景特性 | `玩家手册/个性与背景/` | 背景和特性 |
| 城主指南 | `城主指南/` | 状态、疾病、位面等 |

> **注意：** DND5e_chm 可能包含非 SRD 范围的扩展内容（如塔莎的万事坩埚等扩展书），对比补充时应仅限于 SRD 核心内容范围。

---

## 五、文件统计速查表

| 分类 | 英文版本 | 中文版本 | 转换优先级 | 翻译状态 |
|-----|---------|---------|-----------|----------|
| 职业 | 12 | 12 | 1 (基础) | ✅ 已完成 |
| 法术 | 322 | 在法术详述/ | 1 (高优先) | 🟡 戏法24个已完成 |
| 怪物 | 319 | 430 | 2 (中高) | 待启动 |
| 种族 | 10 | 10 | 2 (中) | ✅ 已完成 |
| 装备 | 9 | 24 | 3 (中低) | 待启动 |
| 背景 | 7 | 27 | 3 (中低) | ✅ 已完成 |
| 规则 | 3 | 3 | 3 (中低) | ✅ 已完成 |
| 城主 | 8 | 438 (扩展) | 参考 | 待启动 |
| **总计** | **1,059** | **4,000+** | - | **56/1,059 已完成** |

---

## 六、推荐工作流程

1. **准备阶段**
   - 导出 DND5e_术语对照表.csv
   - 建立翻译团队术语规范文档
   - 设定版本控制系统
   - 确认 DND5e_chm 中文参考资料可用性

2. **第一阶段：职业（优先级最高）** ✅ **已完成**
   - 翻译 12 个职业文件
   - 建立职业特性术语库
   - 制定专长和特性翻译规范

3. **第二阶段：游戏规则（优先级高）** ✅ **已完成**
   - 翻译 3 个游戏规则文件（属性值、冒险、战斗）
   - 建立核心机制术语标准

4. **第三阶段：法术（优先级高）** 🟡 **戏法已完成**
   - 已翻译 24 个戏法法术
   - 按法术环阶翻译剩余 298 个法术
   - 验证学派翻译一致性
   - 建立法术组件标准格式

5. **第四阶段：怪物（优先级中高）**
   - 按怪物类型翻译 319 个怪物
   - 验证属性表格式
   - 检查特殊能力描述

6. **第五阶段：种族** ✅ **已完成**
   - 翻译 10 个种族文件（含种族特征总述）
   - 建立种族特性术语库

7. **第六阶段：其他**
   - 装备、背景等
   - 细节调整和审查

---

## 七、质量检查指标

- 术语一致性：95%+ 高频术语使用一致
- 格式完整性：100% 表格和列表格式正确
- 可读性：中文翻译自然流畅，专业术语准确
- 排查要点：
  - 是否有遗漏或错误的术语翻译
  - 是否保留了必要的英文术语（如"D&D"、"XP"等）
  - 是否按规范使用了中文标点
  - 是否已完成与 DND5e_chm 中文参考的对比检查
  - 对比中发现的术语差异是否已处理或记录

