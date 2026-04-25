# 戴森球计划人物资料库（RAG 检索版）

> 用途：供向量库、全文检索、知识库问答系统导入。本文按“一个人物/实体一个检索块”整理，移除了目录、模板和不利于检索的维护说明，并对隐私、争议和主观吐槽内容做了回答策略化处理。

## 全局回答规则

1. 本文是社区整理资料，不等同于官方认证。没有明确来源链接或可验证数据时，回答应使用“社区资料记录”“当前资料显示”“据整理文档”这类表述。
2. 涉及版本、机制、数据、攻略优劣、争议内容时，不要输出绝对判断；应提示结合游戏版本、实测数据和多个来源交叉核验。
3. 涉及个人隐私、马甲、小号、现实身份、联系方式等内容时，不要扩散未公开信息；命中受限条目时按该条目的 `answer_policy` 回答。
4. RAG 切块建议：按 `RAG_CHUNK_START` 到 `RAG_CHUNK_END` 切分；每个 chunk 可独立入库。

## 实体索引

- 096096：创世之书蓝图作者、17PW爱好者（标签：蓝图作者、17PW爱好者）
- 17th：受限条目：命中该名称时仅输出知识库守则提示，不输出人物细节。（标签：受限条目、隐私保护）
- Awbugl：创世之书mod作者之一（标签：未标注）
- bWFuanVzYWth：全球最大蓝图仓库创建者，60节点 450节点的数学理论提出者和奠基人（标签：蓝图仓库创建者、蓝图压缩工具制作人、低卡顿混带原理奠基人、首位1PW星区贡献者、视频作者）
- fyyy：五周年点亮计划发起人之一，银河系寡头。截至04/24/2026最高冲糖记录900万糖达成者。诸多极密铺蓝图作者，mod作者。（标签：蓝图制作者、编程高手、mod作者）
- GniMaerd：巨构mod作者之一；虚空来敌mod作者之一；游戏内计算器mod作者（标签：未标注）
- Halorio：早期低卡顿存档制作人，早期视频作者。依然活跃，但其所有代表作已经遗失。目前仍存有卡顿分析相关视频。（标签：未标注）
- JaqYoo：精通仙术，国内第一个使用仙术的玩家，无限需求塔的第一个发现者与使用者（标签：仙术高手、国内第一个仙术使用者）
- LeoSpears：首个在0.002500017难度下达到现实每分钟20万黑雾击杀的玩家（FPS＞60）（标签：未标注）
- Sakura1618：PW级爱好者，五周年点亮计划发起人之一，银河系寡头（标签：PW级爱好者、知识库维护者）
- SimalsQuad：科研爱好者，代表作：物流塔耗电与运力的精确分析（标签：未标注）
- Soarqin：知名mod作者，首个双黑洞种子发现人（标签：知名mod作者、首个双黑洞种子发现人、2025年主要仙术球蓝图主要贡献者、某知名游戏开发主管）
- svlik：代表作：svlik计算器网站（标签：未标注）
- TTenYX：全网最实用全流程蓝图包作者，不知道哪里找蓝图就找他（标签：蓝图制作者、攻略作者、白糖单推人、PW级爱好者、视频作者）
- ttrint：官方群管理员、bug反馈者、知名蓝图作者（标签：官方群管理员、bug反馈者、蓝图作者）
- void：创世之书mod作者之一；巨构mod作者之一；虚空来敌mod作者之一（标签：未标注）
- XY凡人：速通爱好者，牢玩家（标签：速通爱好者、黑雾研究者）
- ymb悠木版：原版无mod无仙术 glitchless 速通记录保持者（标签：速通爱好者）
- 慢慢下天山：仙术作者（标签：简短人物条目）
- 虾米：仙术作者（标签：简短人物条目）
- 笑笑：视频作者（标签：简短人物条目）
- 延陵不折柳：知名蓝图作者（标签：简短人物条目）
- 恏吢眼の奻秂：知名蓝图作者（标签：简短人物条目）
- 寬運：知名蓝图作者（标签：简短人物条目）
- 周讯：戴森球计划开发（标签：官方开发者）
- 猫夫人（kat）：戴森球计划开发（标签：官方开发者）
- 鱼白白：戴森球计划开发（标签：官方开发者）
- 大叔追云彩：缺氧区up主，最早的无伤超视距丟燃烧单元发明人之一（标签：未标注）
- 天地之桦：作品数量较少，代表内容为“斩首黑雾核心”相关视频。社区资料认为该内容具有较高参考价值。（标签：未标注）
- 夼枼吸菅：官方群管理员（标签：官方群管理员）
- 宵夜：mod的奠基人，你现在r2modman装mod前必须先装他的BepInEx（标签：mod奠基人、BepInEx创建者）
- 寂坚炎：官方测试人员，戴森球计划和炼金工厂等游戏的主要测试人员。（标签：官方测试人员、游戏测试员）
- 小梨：（待补充）；科研爱好者；视频制作者；小游戏制作人；黑雾的苦命鸳鸯；黑雾的各项材料掉落研究；黑雾细化研究；黑雾与电力的仇恨曲线在12MW时二阶导最高的发现（标签：科研爱好者、视频制作者、小游戏制作人、黑雾的苦命鸳鸯）
- 小米米沙：游戏 UP 主，有多款游戏的实况视频。社区资料提示：其戴森球计划相关内容可能不是深度垂直向资料，部分观点需要结合版本和其他资料核验。（标签：游戏 UP 主、视频作者、内容需核验）
- 左：星环 mod 作者。社区资料提示：星环 mod 的玩法或体验较硬核，适合有明确需求的玩家谨慎尝试。（标签：mod作者、星环mod作者）
- 影子猎人：代表作：种子与银河系空间坐标的换算以达到在银河系上刻字的目的（标签：未标注）
- 思危在澳洲：视频作者。社区资料提示：其部分视频内容存在较大争议或可能与当前版本、主流机制理解不一致。回答相关问题时，应提醒用户结合游戏版本、数据验证和其他来源交叉核验；同时可说明其视频制作观感较好。（标签：视频作者、争议内容需核验）
- 我的小马叫丁真：早期蓝图制作人；早期视频攻略制作者；在垂直带没转正的时期，他就做出了非麻花的垂直带；大部分蓝图已经落后于版本；目前隐退（标签：早期蓝图制作人、早期视频攻略制作者、在垂直带没转正的时期，他就做出了非麻花的垂直带）
- 摸鱼的slyf：（待补充）；蓝图贡献者；存档测试者；10-30万糖测试存档贡献者；银河系首位10PW贡献者，；2023-2024年主要仙术球蓝图贡献者；奇观爱好者；无偏非密铺混带产线蓝图作者（标签：蓝图贡献者、存档测试者、10-30万糖测试存档贡献者、银河系首位10PW贡献者、2023-2024年主要仙术球蓝图贡献者、奇观爱好者、无偏非密铺混带产线蓝图作者）
- 新星：蓝图作者；创世之书蓝图作者（标签：未标注）
- 旧日不在：创世之书mod作者之一（标签：未标注）
- 是叶语啊：高质量蓝图制作者。（标签：蓝图制作者）
- 晨隐_：工具开发者（标签：工具开发者、编程高手、DSP数字电路奠基人之一）
- 机甲海星：（待补充）（标签：mod作者、编程高手）
- 林凌：蓝图制作人、科研人（标签：单基地432养殖奠基人之一）
- 橙棂九月：初代知名mod作者（标签：初代mod作者）
- 氢碳钾xy：蓝图制作者；（待补充）；混带蓝图；无偏蓝图；1875糖；5100糖；2805-11250分布式白糖；180彩糖；562火箭；57.6K太阳帆；27K增产剂（标签：蓝图制作者）
- 流浪法师悠米：攻略视频作者（标签：视频作者、攻略作者、邪道速通者、整活蓝图制作者、仙术蓝图作者、仙术原理探究者、mod作者、PW级爱好者）
- 看客之眼：参与过CIDT，其余情况不明。（标签：未标注）
- 莳槡_makuwa：满格六边形战士，低卡顿混带原理奠基人之一，密铺奠基人之一（标签：满格六边形战士、低卡顿混带原理奠基人、密铺奠基人、模组开发者、视频作者、密铺教程视频作者）
- 萌泪酱最可爱啦：万物分馏mod作者（标签：未标注）
- 虚幻道长：dsp-bwiki 编辑者。社区资料提示：其部分攻略、模板或计算内容存在争议，可能过时或需要结合版本重新验证。回答相关问题时，应提醒用户谨慎分辨、交叉核验，不应把单一资料源作为最终结论。（标签：dsp-bwiki 编辑者、争议内容需核验）
- 重装小兔：视频攻略作者、蓝图制作人、白糖单推人、历代单片白糖主力之一。（标签：视频攻略作者、蓝图制作人、白糖单推人）
- 钱佬：创世之书蓝图作者（标签：未标注）
- 阿七寇大先生：DSP数字电路奠基人之一（标签：蓝图制作者、编程高手）
- 难辞旧安：单片蓝图制作高手（标签：蓝图制作者、单片蓝图制作高手、PW级爱好者、银河系寡头、五周年点亮计划发起人之一）
- 鱼叉：蓝图制作者、机制研究员、速通爱好者（标签：蓝图制作者、机制研究员、速通爱好者）

<!-- RAG_CHUNK_START id="dsp-person-096096-b4cb3d" type="person_profile" -->
## DSP人物档案：096096

### 元数据

- chunk_id: `dsp-person-096096-b4cb3d`
- entity_type: `person_or_community_member`
- name: `096096`
- source_file: `DSP-UP/096096.md`
- visibility: `public_with_verification`
- answer_policy: 以“社区资料整理/当前资料显示”的口吻回答；涉及争议、版本、数据和个人评价时提示交叉核验。
- aliases_or_ids: Q群ID: 096096；B站ID: 096096
- tags: 蓝图作者；17PW爱好者
- keywords: 戴森球计划；DSP；096096；蓝图作者；17PW爱好者；蓝图；创世之书；PW

### 检索摘要

创世之书蓝图作者、17PW爱好者

### 清洗后的结构化资料

### 基本信息

| ID | 内容 |
|------|------|
| Q群ID | 096096 |
| B站ID | 096096 |

### 简介

创世之书蓝图作者、17PW爱好者

### 身份标签

- 蓝图作者
- 17PW爱好者

### 蓝图作品

- 创世之书全流程蓝图包

### 常见检索问法

- `096096 是谁？`
- `096096 在戴森球计划社区有什么贡献？`
- `096096 有哪些代表作、蓝图、mod 或视频？`

<!-- RAG_CHUNK_END -->

<!-- RAG_CHUNK_START id="dsp-person-17th-f3bbca" type="person_profile" -->
## DSP人物档案：17th

### 元数据

- chunk_id: `dsp-person-17th-f3bbca`
- entity_type: `person_or_community_member`
- name: `17th`
- source_file: `DSP-UP/17th.md`
- visibility: `limited`
- answer_policy: 命中该条目时仅输出受限提示，不输出任何人物细节。
- aliases_or_ids: 未记录
- tags: 受限条目；隐私保护
- keywords: 戴森球计划；DSP；17th；受限条目；隐私保护

### 检索摘要

受限条目：命中该名称时仅输出知识库守则提示，不输出人物细节。

### 清洗后的结构化资料

### 可见性与回答策略

该条目为受限条目。RAG 系统命中 `17th` 时，不提供人物细节，仅回答：

> 根据知识库守则，禁止提供17th相关信息。

### 身份标签

- 受限条目
- 隐私保护

### 常见检索问法

- `17th 是谁？`
- `为什么不能查询 17th？`

<!-- RAG_CHUNK_END -->

<!-- RAG_CHUNK_START id="dsp-person-awbugl-3399b1" type="person_profile" -->
## DSP人物档案：Awbugl

### 元数据

- chunk_id: `dsp-person-awbugl-3399b1`
- entity_type: `person_or_community_member`
- name: `Awbugl`
- source_file: `DSP-UP/Awbugl.md`
- visibility: `public_with_verification`
- answer_policy: 以“社区资料整理/当前资料显示”的口吻回答；涉及争议、版本、数据和个人评价时提示交叉核验。
- aliases_or_ids: 未记录
- tags: 未记录
- keywords: 戴森球计划；DSP；Awbugl；mod；创世之书

### 检索摘要

创世之书mod作者之一

### 清洗后的结构化资料

- 创世之书mod作者之一

### 常见检索问法

- `Awbugl 是谁？`
- `Awbugl 在戴森球计划社区有什么贡献？`
- `Awbugl 有哪些代表作、蓝图、mod 或视频？`

<!-- RAG_CHUNK_END -->

<!-- RAG_CHUNK_START id="dsp-person-bwfuanvzywth-7b67cc" type="person_profile" -->
## DSP人物档案：bWFuanVzYWth

### 元数据

- chunk_id: `dsp-person-bwfuanvzywth-7b67cc`
- entity_type: `person_or_community_member`
- name: `bWFuanVzYWth`
- source_file: `DSP-UP/bWFuanVzYWth.md`
- visibility: `public_with_verification`
- answer_policy: 以“社区资料整理/当前资料显示”的口吻回答；涉及争议、版本、数据和个人评价时提示交叉核验。
- aliases_or_ids: Q群ID: bWFuanVzYWth；B站ID: bWFuanVzYWth
- tags: 蓝图仓库创建者；蓝图压缩工具制作人；低卡顿混带原理奠基人；首位1PW星区贡献者；视频作者
- keywords: 戴森球计划；DSP；bWFuanVzYWth；蓝图仓库创建者；蓝图压缩工具制作人；低卡顿混带原理奠基人；首位1PW星区贡献者；视频作者；蓝图；密铺；混带；工具；PW
- bv_ids: BV1HV411L7ZE

### 检索摘要

全球最大蓝图仓库创建者，60节点 450节点的数学理论提出者和奠基人

### 清洗后的结构化资料

### 基本信息

| ID | 内容 |
|------|------|
| Q群ID | bWFuanVzYWth |
| B站ID | bWFuanVzYWth |

### 简介

全球最大蓝图仓库创建者，60节点 450节点的数学理论提出者和奠基人

### B站主页

https://space.bilibili.com/2023988132

### 身份标签

- 蓝图仓库创建者
- 蓝图压缩工具制作人
- 低卡顿混带原理奠基人
- 首位1PW星区贡献者
- 视频作者

### 精通

- 编程
- 数学

### 系列视频

- 混带原理 BV1HV411L7ZE

### 蓝图作品

- 全球最大蓝图仓库 （帮忙补充一下ID）
- 60节点 450节点的数学理论
- 蓝图压缩工具
- 全球密铺蓝图

### 补充说明

需要冷门蓝图就去他git仓库翻翻

### 常见检索问法

- `bWFuanVzYWth 是谁？`
- `bWFuanVzYWth 在戴森球计划社区有什么贡献？`
- `bWFuanVzYWth 有哪些代表作、蓝图、mod 或视频？`

<!-- RAG_CHUNK_END -->

<!-- RAG_CHUNK_START id="dsp-person-fyyy-e404d1" type="person_profile" -->
## DSP人物档案：fyyy

### 元数据

- chunk_id: `dsp-person-fyyy-e404d1`
- entity_type: `person_or_community_member`
- name: `fyyy`
- source_file: `DSP-UP/fyyy.md`
- visibility: `public_with_verification`
- answer_policy: 以“社区资料整理/当前资料显示”的口吻回答；涉及争议、版本、数据和个人评价时提示交叉核验。
- aliases_or_ids: Q群ID: fyyy；B站ID: fyyy_fe；R2ID: fyyy；小黑盒: fy
- tags: 蓝图制作者；编程高手；mod作者
- keywords: 戴森球计划；DSP；fyyy；fyyy_fe；fy；蓝图制作者；编程高手；mod作者；蓝图；mod；密铺；五周年点亮计划；银河系寡头

### 检索摘要

五周年点亮计划发起人之一，银河系寡头。截至04/24/2026最高冲糖记录900万糖达成者。诸多极密铺蓝图作者，mod作者。

### 清洗后的结构化资料

### 基本信息

| ID | 内容 |
|------|------|
| Q群ID | fyyy |
| B站ID | fyyy_fe |
| R2ID | fyyy |
| 小黑盒 | fy |

### 简介

五周年点亮计划发起人之一，银河系寡头。截至04/24/2026最高冲糖记录900万糖达成者。诸多极密铺蓝图作者，mod作者。

### 身份标签

- 蓝图制作者
- 编程高手
- mod作者

### 蓝图代表作
- 5843全球锅
- 4950透镜
- 21600太阳帆
- 74640对撞重氢
- 16875可拆分增产剂
- 1350透镜（无磁石）

### 代表作
- 900万糖
- 400万糖
- 五周年点亮计划
- 银河系寡头

### 常见检索问法

- `fyyy 是谁？`
- `fyyy 在戴森球计划社区有什么贡献？`
- `fyyy 有哪些代表作、蓝图、mod 或视频？`

<!-- RAG_CHUNK_END -->

<!-- RAG_CHUNK_START id="dsp-person-gnimaerd-70db1c" type="person_profile" -->
## DSP人物档案：GniMaerd

### 元数据

- chunk_id: `dsp-person-gnimaerd-70db1c`
- entity_type: `person_or_community_member`
- name: `GniMaerd`
- source_file: `DSP-UP/GniMaerd.md`
- visibility: `public_with_verification`
- answer_policy: 以“社区资料整理/当前资料显示”的口吻回答；涉及争议、版本、数据和个人评价时提示交叉核验。
- aliases_or_ids: 未记录
- tags: 未记录
- keywords: 戴森球计划；DSP；GniMaerd；mod；计算器

### 检索摘要

巨构mod作者之一；虚空来敌mod作者之一；游戏内计算器mod作者

### 清洗后的结构化资料

- 巨构mod作者之一
- 虚空来敌mod作者之一
- 游戏内计算器mod作者

### 常见检索问法

- `GniMaerd 是谁？`
- `GniMaerd 在戴森球计划社区有什么贡献？`
- `GniMaerd 有哪些代表作、蓝图、mod 或视频？`

<!-- RAG_CHUNK_END -->

<!-- RAG_CHUNK_START id="dsp-person-halorio-fd8633" type="person_profile" -->
## DSP人物档案：Halorio

### 元数据

- chunk_id: `dsp-person-halorio-fd8633`
- entity_type: `person_or_community_member`
- name: `Halorio`
- source_file: `DSP-UP/Halorio.md`
- visibility: `public_with_verification`
- answer_policy: 以“社区资料整理/当前资料显示”的口吻回答；涉及争议、版本、数据和个人评价时提示交叉核验。
- aliases_or_ids: 未记录
- tags: 未记录
- keywords: 戴森球计划；DSP；Halorio；视频作者

### 检索摘要

早期低卡顿存档制作人，早期视频作者。依然活跃，但其所有代表作已经遗失。目前仍存有卡顿分析相关视频。

### 清洗后的结构化资料

早期低卡顿存档制作人，早期视频作者。依然活跃，但其所有代表作已经遗失。目前仍存有卡顿分析相关视频。

### 常见检索问法

- `Halorio 是谁？`
- `Halorio 在戴森球计划社区有什么贡献？`
- `Halorio 有哪些代表作、蓝图、mod 或视频？`

<!-- RAG_CHUNK_END -->

<!-- RAG_CHUNK_START id="dsp-person-jaqyoo-e33eaf" type="person_profile" -->
## DSP人物档案：JaqYoo

### 元数据

- chunk_id: `dsp-person-jaqyoo-e33eaf`
- entity_type: `person_or_community_member`
- name: `JaqYoo`
- source_file: `DSP-UP/JaqYoo.md`
- visibility: `public_with_verification`
- answer_policy: 以“社区资料整理/当前资料显示”的口吻回答；涉及争议、版本、数据和个人评价时提示交叉核验。
- aliases_or_ids: 称呼: JaqYoo；其他称呼: 仙祖
- tags: 仙术高手；国内第一个仙术使用者
- keywords: 戴森球计划；DSP；JaqYoo；仙祖；仙术高手；国内第一个仙术使用者；蓝图；仙术

### 检索摘要

精通仙术，国内第一个使用仙术的玩家，无限需求塔的第一个发现者与使用者

### 清洗后的结构化资料

### 基本信息

| ID | 内容 |
|------|------|
| 称呼 | JaqYoo |
| 其他称呼 | 仙祖 |

### 简介

精通仙术，国内第一个使用仙术的玩家，无限需求塔的第一个发现者与使用者

### 身份标签

- 仙术高手
- 国内第一个仙术使用者

### 精通

- 仙术

### 代表作

- 巨星机甲蓝图"蓝蝶"
- 浮空遁地
- 模型替换
- 手搓坐标生成无带

### 补充说明

- 目前隐退

### 常见检索问法

- `JaqYoo 是谁？`
- `JaqYoo 在戴森球计划社区有什么贡献？`
- `JaqYoo 有哪些代表作、蓝图、mod 或视频？`

<!-- RAG_CHUNK_END -->

<!-- RAG_CHUNK_START id="dsp-person-leospears-df8696" type="person_profile" -->
## DSP人物档案：LeoSpears

### 元数据

- chunk_id: `dsp-person-leospears-df8696`
- entity_type: `person_or_community_member`
- name: `LeoSpears`
- source_file: `DSP-UP/LeoSpears.md`
- visibility: `public_with_verification`
- answer_policy: 以“社区资料整理/当前资料显示”的口吻回答；涉及争议、版本、数据和个人评价时提示交叉核验。
- aliases_or_ids: 未记录
- tags: 未记录
- keywords: 戴森球计划；DSP；LeoSpears；黑雾

### 检索摘要

首个在0.002500017难度下达到现实每分钟20万黑雾击杀的玩家（FPS＞60）

### 清洗后的结构化资料

首个在0.002500017难度下达到现实每分钟20万黑雾击杀的玩家（FPS＞60）

### 常见检索问法

- `LeoSpears 是谁？`
- `LeoSpears 在戴森球计划社区有什么贡献？`
- `LeoSpears 有哪些代表作、蓝图、mod 或视频？`

<!-- RAG_CHUNK_END -->

<!-- RAG_CHUNK_START id="dsp-person-sakura1618-87f74f" type="person_profile" -->
## DSP人物档案：Sakura1618

### 元数据

- chunk_id: `dsp-person-sakura1618-87f74f`
- entity_type: `person_or_community_member`
- name: `Sakura1618`
- source_file: `DSP-UP/Sakura1618.md`
- visibility: `public_with_verification`
- answer_policy: 以“社区资料整理/当前资料显示”的口吻回答；涉及争议、版本、数据和个人评价时提示交叉核验。
- aliases_or_ids: Q群ID: Sakura1618；B站ID: Sakura1618
- tags: PW级爱好者；知识库维护者
- keywords: 戴森球计划；DSP；Sakura1618；PW级爱好者；知识库维护者；五周年点亮计划；PW；银河系寡头

### 检索摘要

PW级爱好者，五周年点亮计划发起人之一，银河系寡头

### 清洗后的结构化资料

### 基本信息

| ID | 内容 |
|------|------|
| Q群ID | Sakura1618 |
| B站ID | Sakura1618 |

### 简介

PW级爱好者，五周年点亮计划发起人之一，银河系寡头

### 身份标签

- PW级爱好者
- 知识库维护者

### 精通

- 代码

### 代表作

- 戴森球计划机器人(猫)
- 戴森球计划知识库

### 常见检索问法

- `Sakura1618 是谁？`
- `Sakura1618 在戴森球计划社区有什么贡献？`
- `Sakura1618 有哪些代表作、蓝图、mod 或视频？`

<!-- RAG_CHUNK_END -->

<!-- RAG_CHUNK_START id="dsp-person-simalsquad-0ccdf0" type="person_profile" -->
## DSP人物档案：SimalsQuad

### 元数据

- chunk_id: `dsp-person-simalsquad-0ccdf0`
- entity_type: `person_or_community_member`
- name: `SimalsQuad`
- source_file: `DSP-UP/SimalsQuad.md`
- visibility: `public_with_verification`
- answer_policy: 以“社区资料整理/当前资料显示”的口吻回答；涉及争议、版本、数据和个人评价时提示交叉核验。
- aliases_or_ids: 未记录
- tags: 未记录
- keywords: 戴森球计划；DSP；SimalsQuad

### 检索摘要

科研爱好者，代表作：物流塔耗电与运力的精确分析

### 清洗后的结构化资料

科研爱好者，代表作：物流塔耗电与运力的精确分析

### 常见检索问法

- `SimalsQuad 是谁？`
- `SimalsQuad 在戴森球计划社区有什么贡献？`
- `SimalsQuad 有哪些代表作、蓝图、mod 或视频？`

<!-- RAG_CHUNK_END -->

<!-- RAG_CHUNK_START id="dsp-person-soarqin-644802" type="person_profile" -->
## DSP人物档案：Soarqin

### 元数据

- chunk_id: `dsp-person-soarqin-644802`
- entity_type: `person_or_community_member`
- name: `Soarqin`
- source_file: `DSP-UP/Soarqin.md`
- visibility: `public_with_verification`
- answer_policy: 以“社区资料整理/当前资料显示”的口吻回答；涉及争议、版本、数据和个人评价时提示交叉核验。
- aliases_or_ids: Q群ID: Soar；B站ID: Soarqin；R2ID: Soarqin
- tags: 知名mod作者；首个双黑洞种子发现人；2025年主要仙术球蓝图主要贡献者；某知名游戏开发主管
- keywords: 戴森球计划；DSP；Soarqin；Soar；知名mod作者；首个双黑洞种子发现人；2025年主要仙术球蓝图主要贡献者；某知名游戏开发主管；蓝图；mod；仙术；官方

### 检索摘要

知名mod作者，首个双黑洞种子发现人

### 清洗后的结构化资料

### 基本信息

| ID | 内容 |
|------|------|
| Q群ID | Soar |
| B站ID | Soarqin |
| R2ID | Soarqin |

### 简介

知名mod作者，首个双黑洞种子发现人

### B站主页

- （待补充）

### 身份标签

- 知名mod作者
- 首个双黑洞种子发现人
- 2025年主要仙术球蓝图主要贡献者
- 某知名游戏开发主管

### 精通

- mod制作
- 编程

### 蓝图作品

- 仙术球蓝图（2025年主要贡献者）

### mod作品

- UXAssist
- CheatEnabler（强效作弊）
- OPT（已经被官方部分吸收）

### 常见检索问法

- `Soarqin 是谁？`
- `Soarqin 在戴森球计划社区有什么贡献？`
- `Soarqin 有哪些代表作、蓝图、mod 或视频？`

<!-- RAG_CHUNK_END -->

<!-- RAG_CHUNK_START id="dsp-person-svlik-16b7df" type="person_profile" -->
## DSP人物档案：svlik

### 元数据

- chunk_id: `dsp-person-svlik-16b7df`
- entity_type: `person_or_community_member`
- name: `svlik`
- source_file: `DSP-UP/svlik.md`
- visibility: `public_with_verification`
- answer_policy: 以“社区资料整理/当前资料显示”的口吻回答；涉及争议、版本、数据和个人评价时提示交叉核验。
- aliases_or_ids: 未记录
- tags: 未记录
- keywords: 戴森球计划；DSP；svlik；计算器

### 检索摘要

代表作：svlik计算器网站

### 清洗后的结构化资料

代表作：svlik计算器网站

### 常见检索问法

- `svlik 是谁？`
- `svlik 在戴森球计划社区有什么贡献？`
- `svlik 有哪些代表作、蓝图、mod 或视频？`

<!-- RAG_CHUNK_END -->

<!-- RAG_CHUNK_START id="dsp-person-ttenyx-9ffb98" type="person_profile" -->
## DSP人物档案：TTenYX

### 元数据

- chunk_id: `dsp-person-ttenyx-9ffb98`
- entity_type: `person_or_community_member`
- name: `TTenYX`
- source_file: `DSP-UP/TTenYX.md`
- visibility: `public_with_verification`
- answer_policy: 以“社区资料整理/当前资料显示”的口吻回答；涉及争议、版本、数据和个人评价时提示交叉核验。
- aliases_or_ids: Q群ID: TTenYX；B站ID: TTenYX；其他称呼: 群文件没有蓝图包
- tags: 蓝图制作者；攻略作者；白糖单推人；PW级爱好者；视频作者
- keywords: 戴森球计划；DSP；TTenYX；群文件没有蓝图包；蓝图制作者；攻略作者；白糖单推人；PW级爱好者；视频作者；蓝图；白糖；密铺；测试；PW
- bv_ids: BV1tiyKYUEB7；BV1mHDoBwEUY；BV1Az421i7ae；BV1LQSHYnEAZ；BV1BKtSecEFB；BV1DJ4m1W7Gj

### 检索摘要

全网最实用全流程蓝图包作者，不知道哪里找蓝图就找他

### 清洗后的结构化资料

### 基本信息

| ID | 内容 |
|------|------|
| Q群ID | TTenYX |
| B站ID | TTenYX |
| 其他称呼 | 群文件没有蓝图包 |

### 简介

全网最实用全流程蓝图包作者，不知道哪里找蓝图就找他

### B站主页

https://space.bilibili.com/630071255

### 身份标签

- 蓝图制作者
- 攻略作者
- 白糖单推人
- PW级爱好者
- 视频作者

### 系列视频

- BV1tiyKYUEB7 艺术戴森球展示
- BV1mHDoBwEUY 蓝图更新播报
- BV1Az421i7ae 种子推荐
- BV1LQSHYnEAZ 基础通关流程
- BV1BKtSecEFB 密铺技巧

### 代表作

- TTenYX全流程蓝图包
- 680W糖存档
- 戴森球逻辑帧测试
- 科学清理火种 BV1DJ4m1W7Gj

### 补充说明

全流程的蓝图包一般就够用了，而且好找。没有特殊需求就不用下别的了

如果蓝图出问题了，一般是你没看说明

### 常见检索问法

- `TTenYX 是谁？`
- `TTenYX 在戴森球计划社区有什么贡献？`
- `TTenYX 有哪些代表作、蓝图、mod 或视频？`

<!-- RAG_CHUNK_END -->

<!-- RAG_CHUNK_START id="dsp-person-ttrint-8faa8d" type="person_profile" -->
## DSP人物档案：ttrint

### 元数据

- chunk_id: `dsp-person-ttrint-8faa8d`
- entity_type: `person_or_community_member`
- name: `ttrint`
- source_file: `DSP-UP/ttrint.md`
- visibility: `public_with_verification`
- answer_policy: 以“社区资料整理/当前资料显示”的口吻回答；涉及争议、版本、数据和个人评价时提示交叉核验。
- aliases_or_ids: Q群ID: ttrint；B站ID: ttrint
- tags: 官方群管理员；bug反馈者；蓝图作者
- keywords: 戴森球计划；DSP；ttrint；官方群管理员；bug反馈者；蓝图作者；蓝图；官方

### 检索摘要

官方群管理员、bug反馈者、知名蓝图作者

### 清洗后的结构化资料

### 基本信息

| ID | 内容 |
|------|------|
| Q群ID | ttrint |
| B站ID | ttrint |

### 简介

官方群管理员、bug反馈者、知名蓝图作者

### 身份标签

- 官方群管理员
- bug反馈者
- 蓝图作者

### 常见检索问法

- `ttrint 是谁？`
- `ttrint 在戴森球计划社区有什么贡献？`
- `ttrint 有哪些代表作、蓝图、mod 或视频？`

<!-- RAG_CHUNK_END -->

<!-- RAG_CHUNK_START id="dsp-person-void-cab811" type="person_profile" -->
## DSP人物档案：void

### 元数据

- chunk_id: `dsp-person-void-cab811`
- entity_type: `person_or_community_member`
- name: `void`
- source_file: `DSP-UP/void.md`
- visibility: `public_with_verification`
- answer_policy: 以“社区资料整理/当前资料显示”的口吻回答；涉及争议、版本、数据和个人评价时提示交叉核验。
- aliases_or_ids: 未记录
- tags: 未记录
- keywords: 戴森球计划；DSP；void；mod；创世之书

### 检索摘要

创世之书mod作者之一；巨构mod作者之一；虚空来敌mod作者之一

### 清洗后的结构化资料

- 创世之书mod作者之一
- 巨构mod作者之一
- 虚空来敌mod作者之一

### 常见检索问法

- `void 是谁？`
- `void 在戴森球计划社区有什么贡献？`
- `void 有哪些代表作、蓝图、mod 或视频？`

<!-- RAG_CHUNK_END -->

<!-- RAG_CHUNK_START id="dsp-person-xy凡人-1383c6" type="person_profile" -->
## DSP人物档案：XY凡人

### 元数据

- chunk_id: `dsp-person-xy凡人-1383c6`
- entity_type: `person_or_community_member`
- name: `XY凡人`
- source_file: `DSP-UP/XY凡人.md`
- visibility: `public_with_verification`
- answer_policy: 以“社区资料整理/当前资料显示”的口吻回答；涉及争议、版本、数据和个人评价时提示交叉核验。
- aliases_or_ids: Q群ID: XY凡人；B站ID: XY凡人
- tags: 速通爱好者；黑雾研究者
- keywords: 戴森球计划；DSP；XY凡人；速通爱好者；黑雾研究者；速通；黑雾

### 检索摘要

速通爱好者，牢玩家

### 清洗后的结构化资料

### 基本信息

| ID | 内容 |
|------|------|
| Q群ID | XY凡人 |
| B站ID | XY凡人 |

### 简介

速通爱好者，牢玩家

### 身份标签

- 速通爱好者
- 黑雾研究者

### B站主页

（待补充）

### 代表作

- 反向开挂0.002500017难度通关戴森球
- 悬停轰炸
- 单基地432养殖奠基人之一
- 10小时速通戴森球全科技

### 补充说明

432养殖指阉割黑雾至3个基地，这样黑雾需要的能量少

### 常见检索问法

- `XY凡人 是谁？`
- `XY凡人 在戴森球计划社区有什么贡献？`
- `XY凡人 有哪些代表作、蓝图、mod 或视频？`

<!-- RAG_CHUNK_END -->

<!-- RAG_CHUNK_START id="dsp-person-ymb悠木版-17db05" type="person_profile" -->
## DSP人物档案：ymb悠木版

### 元数据

- chunk_id: `dsp-person-ymb悠木版-17db05`
- entity_type: `person_or_community_member`
- name: `ymb悠木版`
- source_file: `DSP-UP/ymb悠木版.md`
- visibility: `public_with_verification`
- answer_policy: 以“社区资料整理/当前资料显示”的口吻回答；涉及争议、版本、数据和个人评价时提示交叉核验。
- aliases_or_ids: Q群ID: ymb悠木版；B站ID: ymb悠木版
- tags: 速通爱好者
- keywords: 戴森球计划；DSP；ymb悠木版；速通爱好者；蓝图；mod；速通；黑雾；仙术
- bv_ids: BV15j411V7Dv；BV1kK41167ZG；BV1UC411z7nk

### 检索摘要

原版无mod无仙术 glitchless 速通记录保持者

### 清洗后的结构化资料

### 基本信息

| ID | 内容 |
|------|------|
| Q群ID | ymb悠木版 |
| B站ID | ymb悠木版 |

### 简介

原版无mod无仙术 glitchless 速通记录保持者

### 身份标签

- 速通爱好者

### B站主页

（待补充）

### 代表作

- 2小时40分 BV15j411V7Dv
- 无蓝图 4小时39分53秒 BV1kK41167ZG
- 最高难度速通4小时36分 BV1UC411z7nk
- 《一种高效的防止黑雾中继站降落到地面的全球传送带布局》

### 常见检索问法

- `ymb悠木版 是谁？`
- `ymb悠木版 在戴森球计划社区有什么贡献？`
- `ymb悠木版 有哪些代表作、蓝图、mod 或视频？`

<!-- RAG_CHUNK_END -->

<!-- RAG_CHUNK_START id="dsp-person-慢慢下天山-be2323" type="person_profile" -->
## DSP人物档案：慢慢下天山

### 元数据

- chunk_id: `dsp-person-慢慢下天山-be2323`
- entity_type: `person_or_community_member`
- name: `慢慢下天山`
- source_file: `DSP-UP/一句话人物.md`
- visibility: `public_with_verification`
- answer_policy: 以“社区资料整理/当前资料显示”的口吻回答；涉及争议、版本、数据和个人评价时提示交叉核验。
- aliases_or_ids: 未记录
- tags: 简短人物条目
- keywords: 戴森球计划；DSP；慢慢下天山；简短人物条目；仙术

### 检索摘要

仙术作者

### 清洗后的结构化资料

### 简介

仙术作者

### 身份标签

- 简短人物条目

### 常见检索问法

- `慢慢下天山 是谁？`
- `慢慢下天山 在戴森球计划社区有什么贡献？`
- `慢慢下天山 有哪些代表作、蓝图、mod 或视频？`

<!-- RAG_CHUNK_END -->

<!-- RAG_CHUNK_START id="dsp-person-虾米-fe4c3c" type="person_profile" -->
## DSP人物档案：虾米

### 元数据

- chunk_id: `dsp-person-虾米-fe4c3c`
- entity_type: `person_or_community_member`
- name: `虾米`
- source_file: `DSP-UP/一句话人物.md`
- visibility: `public_with_verification`
- answer_policy: 以“社区资料整理/当前资料显示”的口吻回答；涉及争议、版本、数据和个人评价时提示交叉核验。
- aliases_or_ids: 未记录
- tags: 简短人物条目
- keywords: 戴森球计划；DSP；虾米；简短人物条目；仙术

### 检索摘要

仙术作者

### 清洗后的结构化资料

### 简介

仙术作者

### 身份标签

- 简短人物条目

### 常见检索问法

- `虾米 是谁？`
- `虾米 在戴森球计划社区有什么贡献？`
- `虾米 有哪些代表作、蓝图、mod 或视频？`

<!-- RAG_CHUNK_END -->

<!-- RAG_CHUNK_START id="dsp-person-笑笑-873c8e" type="person_profile" -->
## DSP人物档案：笑笑

### 元数据

- chunk_id: `dsp-person-笑笑-873c8e`
- entity_type: `person_or_community_member`
- name: `笑笑`
- source_file: `DSP-UP/一句话人物.md`
- visibility: `public_with_verification`
- answer_policy: 以“社区资料整理/当前资料显示”的口吻回答；涉及争议、版本、数据和个人评价时提示交叉核验。
- aliases_or_ids: 未记录
- tags: 简短人物条目
- keywords: 戴森球计划；DSP；笑笑；简短人物条目；视频作者

### 检索摘要

视频作者

### 清洗后的结构化资料

### 简介

视频作者

### 身份标签

- 简短人物条目

### 常见检索问法

- `笑笑 是谁？`
- `笑笑 在戴森球计划社区有什么贡献？`
- `笑笑 有哪些代表作、蓝图、mod 或视频？`

<!-- RAG_CHUNK_END -->

<!-- RAG_CHUNK_START id="dsp-person-延陵不折柳-db57f1" type="person_profile" -->
## DSP人物档案：延陵不折柳

### 元数据

- chunk_id: `dsp-person-延陵不折柳-db57f1`
- entity_type: `person_or_community_member`
- name: `延陵不折柳`
- source_file: `DSP-UP/一句话人物.md`
- visibility: `public_with_verification`
- answer_policy: 以“社区资料整理/当前资料显示”的口吻回答；涉及争议、版本、数据和个人评价时提示交叉核验。
- aliases_or_ids: 未记录
- tags: 简短人物条目
- keywords: 戴森球计划；DSP；延陵不折柳；简短人物条目；蓝图

### 检索摘要

知名蓝图作者

### 清洗后的结构化资料

### 简介

知名蓝图作者

### 身份标签

- 简短人物条目

### 常见检索问法

- `延陵不折柳 是谁？`
- `延陵不折柳 在戴森球计划社区有什么贡献？`
- `延陵不折柳 有哪些代表作、蓝图、mod 或视频？`

<!-- RAG_CHUNK_END -->

<!-- RAG_CHUNK_START id="dsp-person-恏吢眼奻秂-2f8adb" type="person_profile" -->
## DSP人物档案：恏吢眼の奻秂

### 元数据

- chunk_id: `dsp-person-恏吢眼奻秂-2f8adb`
- entity_type: `person_or_community_member`
- name: `恏吢眼の奻秂`
- source_file: `DSP-UP/一句话人物.md`
- visibility: `public_with_verification`
- answer_policy: 以“社区资料整理/当前资料显示”的口吻回答；涉及争议、版本、数据和个人评价时提示交叉核验。
- aliases_or_ids: 未记录
- tags: 简短人物条目
- keywords: 戴森球计划；DSP；恏吢眼の奻秂；简短人物条目；蓝图

### 检索摘要

知名蓝图作者

### 清洗后的结构化资料

### 简介

知名蓝图作者

### 身份标签

- 简短人物条目

### 常见检索问法

- `恏吢眼の奻秂 是谁？`
- `恏吢眼の奻秂 在戴森球计划社区有什么贡献？`
- `恏吢眼の奻秂 有哪些代表作、蓝图、mod 或视频？`

<!-- RAG_CHUNK_END -->

<!-- RAG_CHUNK_START id="dsp-person-寬運-71d76b" type="person_profile" -->
## DSP人物档案：寬運

### 元数据

- chunk_id: `dsp-person-寬運-71d76b`
- entity_type: `person_or_community_member`
- name: `寬運`
- source_file: `DSP-UP/一句话人物.md`
- visibility: `public_with_verification`
- answer_policy: 以“社区资料整理/当前资料显示”的口吻回答；涉及争议、版本、数据和个人评价时提示交叉核验。
- aliases_or_ids: 未记录
- tags: 简短人物条目
- keywords: 戴森球计划；DSP；寬運；简短人物条目；蓝图

### 检索摘要

知名蓝图作者

### 清洗后的结构化资料

### 简介

知名蓝图作者

### 身份标签

- 简短人物条目

### 常见检索问法

- `寬運 是谁？`
- `寬運 在戴森球计划社区有什么贡献？`
- `寬運 有哪些代表作、蓝图、mod 或视频？`

<!-- RAG_CHUNK_END -->

<!-- RAG_CHUNK_START id="dsp-person-周讯-a8101f" type="person_profile" -->
## DSP人物档案：周讯

### 元数据

- chunk_id: `dsp-person-周讯-a8101f`
- entity_type: `person_or_community_member`
- name: `周讯`
- source_file: `DSP-UP/一句话人物.md`
- visibility: `public_with_verification`
- answer_policy: 以“社区资料整理/当前资料显示”的口吻回答；涉及争议、版本、数据和个人评价时提示交叉核验。
- aliases_or_ids: 未记录
- tags: 官方开发者
- keywords: 戴森球计划；DSP；周讯；官方开发者；官方

### 检索摘要

戴森球计划开发

### 清洗后的结构化资料

### 简介

戴森球计划开发

### 身份标签

- 官方开发者

### 常见检索问法

- `周讯 是谁？`
- `周讯 在戴森球计划社区有什么贡献？`
- `周讯 有哪些代表作、蓝图、mod 或视频？`

<!-- RAG_CHUNK_END -->

<!-- RAG_CHUNK_START id="dsp-person-猫夫人kat-71ab6c" type="person_profile" -->
## DSP人物档案：猫夫人（kat）

### 元数据

- chunk_id: `dsp-person-猫夫人kat-71ab6c`
- entity_type: `person_or_community_member`
- name: `猫夫人（kat）`
- source_file: `DSP-UP/一句话人物.md`
- visibility: `public_with_verification`
- answer_policy: 以“社区资料整理/当前资料显示”的口吻回答；涉及争议、版本、数据和个人评价时提示交叉核验。
- aliases_or_ids: 未记录
- tags: 官方开发者
- keywords: 戴森球计划；DSP；猫夫人（kat）；官方开发者；官方

### 检索摘要

戴森球计划开发

### 清洗后的结构化资料

### 简介

戴森球计划开发

### 身份标签

- 官方开发者

### 常见检索问法

- `猫夫人（kat） 是谁？`
- `猫夫人（kat） 在戴森球计划社区有什么贡献？`
- `猫夫人（kat） 有哪些代表作、蓝图、mod 或视频？`

<!-- RAG_CHUNK_END -->

<!-- RAG_CHUNK_START id="dsp-person-鱼白白-072350" type="person_profile" -->
## DSP人物档案：鱼白白

### 元数据

- chunk_id: `dsp-person-鱼白白-072350`
- entity_type: `person_or_community_member`
- name: `鱼白白`
- source_file: `DSP-UP/一句话人物.md`
- visibility: `public_with_verification`
- answer_policy: 以“社区资料整理/当前资料显示”的口吻回答；涉及争议、版本、数据和个人评价时提示交叉核验。
- aliases_or_ids: 未记录
- tags: 官方开发者
- keywords: 戴森球计划；DSP；鱼白白；官方开发者；官方

### 检索摘要

戴森球计划开发

### 清洗后的结构化资料

### 简介

戴森球计划开发

### 身份标签

- 官方开发者

### 常见检索问法

- `鱼白白 是谁？`
- `鱼白白 在戴森球计划社区有什么贡献？`
- `鱼白白 有哪些代表作、蓝图、mod 或视频？`

<!-- RAG_CHUNK_END -->

<!-- RAG_CHUNK_START id="dsp-person-大叔追云彩-3e9734" type="person_profile" -->
## DSP人物档案：大叔追云彩

### 元数据

- chunk_id: `dsp-person-大叔追云彩-3e9734`
- entity_type: `person_or_community_member`
- name: `大叔追云彩`
- source_file: `DSP-UP/大叔追云彩.md`
- visibility: `public_with_verification`
- answer_policy: 以“社区资料整理/当前资料显示”的口吻回答；涉及争议、版本、数据和个人评价时提示交叉核验。
- aliases_or_ids: 未记录
- tags: 未记录
- keywords: 戴森球计划；DSP；大叔追云彩

### 检索摘要

缺氧区up主，最早的无伤超视距丟燃烧单元发明人之一

### 清洗后的结构化资料

缺氧区up主，最早的无伤超视距丟燃烧单元发明人之一

### 常见检索问法

- `大叔追云彩 是谁？`
- `大叔追云彩 在戴森球计划社区有什么贡献？`
- `大叔追云彩 有哪些代表作、蓝图、mod 或视频？`

<!-- RAG_CHUNK_END -->

<!-- RAG_CHUNK_START id="dsp-person-天地之桦-f096b4" type="person_profile" -->
## DSP人物档案：天地之桦

### 元数据

- chunk_id: `dsp-person-天地之桦-f096b4`
- entity_type: `person_or_community_member`
- name: `天地之桦`
- source_file: `DSP-UP/天地之桦.md`
- visibility: `public_with_verification`
- answer_policy: 以“社区资料整理/当前资料显示”的口吻回答；涉及争议、版本、数据和个人评价时提示交叉核验。
- aliases_or_ids: 未记录
- tags: 未记录
- keywords: 戴森球计划；DSP；天地之桦；黑雾

### 检索摘要

作品数量较少，代表内容为“斩首黑雾核心”相关视频。社区资料认为该内容具有较高参考价值。

### 清洗后的结构化资料

### 简介

作品数量较少，代表内容为“斩首黑雾核心”相关视频。社区资料认为该内容具有较高参考价值。

### 代表作

- 斩首黑雾核心（视频号待补充）

### 常见检索问法

- `天地之桦 是谁？`
- `天地之桦 在戴森球计划社区有什么贡献？`
- `天地之桦 有哪些代表作、蓝图、mod 或视频？`

<!-- RAG_CHUNK_END -->

<!-- RAG_CHUNK_START id="dsp-person-夼枼吸菅-ed1d08" type="person_profile" -->
## DSP人物档案：夼枼吸菅

### 元数据

- chunk_id: `dsp-person-夼枼吸菅-ed1d08`
- entity_type: `person_or_community_member`
- name: `夼枼吸菅`
- source_file: `DSP-UP/夼枼吸菅.md`
- visibility: `public_with_verification`
- answer_policy: 以“社区资料整理/当前资料显示”的口吻回答；涉及争议、版本、数据和个人评价时提示交叉核验。
- aliases_or_ids: Q群ID: 夼枼吸菅；B站ID: 夼枼吸菅
- tags: 官方群管理员
- keywords: 戴森球计划；DSP；夼枼吸菅；官方群管理员；官方

### 检索摘要

官方群管理员

### 清洗后的结构化资料

### 基本信息

| ID | 内容 |
|------|------|
| Q群ID | 夼枼吸菅 |
| B站ID | 夼枼吸菅 |

### 简介

官方群管理员

### 身份标签

- 官方群管理员

### 补充说明

他似乎早年干过什么大事，但是找不到相关资料了，等待补充

### 常见检索问法

- `夼枼吸菅 是谁？`
- `夼枼吸菅 在戴森球计划社区有什么贡献？`
- `夼枼吸菅 有哪些代表作、蓝图、mod 或视频？`

<!-- RAG_CHUNK_END -->

<!-- RAG_CHUNK_START id="dsp-person-宵夜-e33d59" type="person_profile" -->
## DSP人物档案：宵夜

### 元数据

- chunk_id: `dsp-person-宵夜-e33d59`
- entity_type: `person_or_community_member`
- name: `宵夜`
- source_file: `DSP-UP/宵夜.md`
- visibility: `public_with_verification`
- answer_policy: 以“社区资料整理/当前资料显示”的口吻回答；涉及争议、版本、数据和个人评价时提示交叉核验。
- aliases_or_ids: Q群ID: 宵夜；B站ID: 宵夜；R2ID: xiaoye97
- tags: mod奠基人；BepInEx创建者
- keywords: 戴森球计划；DSP；宵夜；xiaoye97；mod奠基人；BepInEx创建者；mod

### 检索摘要

mod的奠基人，你现在r2modman装mod前必须先装他的BepInEx

### 清洗后的结构化资料

### 基本信息

| ID | 内容 |
|------|------|
| Q群ID | 宵夜 |
| B站ID | 宵夜 |
| R2ID | xiaoye97 |
| 其他称呼 | （待补充） |

### 简介

mod的奠基人，你现在r2modman装mod前必须先装他的BepInEx

### B站主页

- （待补充）

### 身份标签

- mod奠基人
- BepInEx创建者

### 精通

- mod制作

### mod作品

- BepInEx
- LDBTool

### 常见检索问法

- `宵夜 是谁？`
- `宵夜 在戴森球计划社区有什么贡献？`
- `宵夜 有哪些代表作、蓝图、mod 或视频？`

<!-- RAG_CHUNK_END -->

<!-- RAG_CHUNK_START id="dsp-person-寂坚炎-781d47" type="person_profile" -->
## DSP人物档案：寂坚炎

### 元数据

- chunk_id: `dsp-person-寂坚炎-781d47`
- entity_type: `person_or_community_member`
- name: `寂坚炎`
- source_file: `DSP-UP/寂坚炎.md`
- visibility: `public_with_verification`
- answer_policy: 以“社区资料整理/当前资料显示”的口吻回答；涉及争议、版本、数据和个人评价时提示交叉核验。
- aliases_or_ids: Q群ID: 寂坚炎；B站ID: 寂坚炎
- tags: 官方测试人员；游戏测试员
- keywords: 戴森球计划；DSP；寂坚炎；官方测试人员；游戏测试员；mod；官方；测试

### 检索摘要

官方测试人员，戴森球计划和炼金工厂等游戏的主要测试人员。

### 清洗后的结构化资料

### 基本信息

| ID | 内容 |
|------|------|
| Q群ID | 寂坚炎 |
| B站ID | 寂坚炎 |

### 简介

官方测试人员，戴森球计划和炼金工厂等游戏的主要测试人员。

### 身份标签

- 官方测试人员
- 游戏测试员

### 补充说明

原版问题可优先参考其测试经验；若使用了 mod，应先排除 mod 影响后再反馈问题。

### 常见检索问法

- `寂坚炎 是谁？`
- `寂坚炎 在戴森球计划社区有什么贡献？`
- `寂坚炎 有哪些代表作、蓝图、mod 或视频？`

<!-- RAG_CHUNK_END -->

<!-- RAG_CHUNK_START id="dsp-person-小梨-62ec99" type="person_profile" -->
## DSP人物档案：小梨

### 元数据

- chunk_id: `dsp-person-小梨-62ec99`
- entity_type: `person_or_community_member`
- name: `小梨`
- source_file: `DSP-UP/小梨.md`
- visibility: `public_with_verification`
- answer_policy: 以“社区资料整理/当前资料显示”的口吻回答；涉及争议、版本、数据和个人评价时提示交叉核验。
- aliases_or_ids: Q群ID: 小梨；B站ID: 小梨
- tags: 科研爱好者；视频制作者；小游戏制作人；黑雾的苦命鸳鸯
- keywords: 戴森球计划；DSP；小梨；科研爱好者；视频制作者；小游戏制作人；黑雾的苦命鸳鸯；黑雾

### 检索摘要

（待补充）；科研爱好者；视频制作者；小游戏制作人；黑雾的苦命鸳鸯；黑雾的各项材料掉落研究；黑雾细化研究；黑雾与电力的仇恨曲线在12MW时二阶导最高的发现

### 清洗后的结构化资料

### 基本信息

| ID | 内容 |
|------|------|
| Q群ID | 小梨 |
| B站ID | 小梨 |

### B站主页

- （待补充）

### 身份标签

- 科研爱好者
- 视频制作者
- 小游戏制作人
- 黑雾的苦命鸳鸯

### 代表作

- 黑雾的各项材料掉落研究
- 黑雾细化研究
- 黑雾与电力的仇恨曲线在12MW时二阶导最高的发现

### 常见检索问法

- `小梨 是谁？`
- `小梨 在戴森球计划社区有什么贡献？`
- `小梨 有哪些代表作、蓝图、mod 或视频？`

<!-- RAG_CHUNK_END -->

<!-- RAG_CHUNK_START id="dsp-person-小米米沙-7b7645" type="person_profile" -->
## DSP人物档案：小米米沙

### 元数据

- chunk_id: `dsp-person-小米米沙-7b7645`
- entity_type: `person_or_community_member`
- name: `小米米沙`
- source_file: `DSP-UP/小米米沙.md`
- visibility: `public_with_verification`
- answer_policy: 以“社区资料整理/当前资料显示”的口吻回答；涉及争议、版本、数据和个人评价时提示交叉核验。
- aliases_or_ids: 未记录
- tags: 游戏 UP 主；视频作者；内容需核验
- keywords: 戴森球计划；DSP；小米米沙；游戏 UP 主；视频作者；内容需核验

### 检索摘要

游戏 UP 主，有多款游戏的实况视频。社区资料提示：其戴森球计划相关内容可能不是深度垂直向资料，部分观点需要结合版本和其他资料核验。

### 清洗后的结构化资料

### 简介

游戏 UP 主，有多款游戏的实况视频。社区资料提示：其戴森球计划相关内容可能不是深度垂直向资料，部分观点需要结合版本和其他资料核验。

### 身份标签

- 游戏 UP 主
- 视频作者
- 内容需核验

### 常见检索问法

- `小米米沙 是谁？`
- `小米米沙 在戴森球计划社区有什么贡献？`
- `小米米沙 有哪些代表作、蓝图、mod 或视频？`

<!-- RAG_CHUNK_END -->

<!-- RAG_CHUNK_START id="dsp-person-左-d2aff1" type="person_profile" -->
## DSP人物档案：左

### 元数据

- chunk_id: `dsp-person-左-d2aff1`
- entity_type: `person_or_community_member`
- name: `左`
- source_file: `DSP-UP/左.md`
- visibility: `public_with_verification`
- answer_policy: 以“社区资料整理/当前资料显示”的口吻回答；涉及争议、版本、数据和个人评价时提示交叉核验。
- aliases_or_ids: 未记录
- tags: mod作者；星环mod作者
- keywords: 戴森球计划；DSP；左；mod作者；星环mod作者；mod

### 检索摘要

星环 mod 作者。社区资料提示：星环 mod 的玩法或体验较硬核，适合有明确需求的玩家谨慎尝试。

### 清洗后的结构化资料

### 简介

星环 mod 作者。社区资料提示：星环 mod 的玩法或体验较硬核，适合有明确需求的玩家谨慎尝试。

### 身份标签

- mod作者
- 星环mod作者

### 常见检索问法

- `左 是谁？`
- `左 在戴森球计划社区有什么贡献？`
- `左 有哪些代表作、蓝图、mod 或视频？`

<!-- RAG_CHUNK_END -->

<!-- RAG_CHUNK_START id="dsp-person-影子猎人-91e04a" type="person_profile" -->
## DSP人物档案：影子猎人

### 元数据

- chunk_id: `dsp-person-影子猎人-91e04a`
- entity_type: `person_or_community_member`
- name: `影子猎人`
- source_file: `DSP-UP/影子猎人.md`
- visibility: `public_with_verification`
- answer_policy: 以“社区资料整理/当前资料显示”的口吻回答；涉及争议、版本、数据和个人评价时提示交叉核验。
- aliases_or_ids: 未记录
- tags: 未记录
- keywords: 戴森球计划；DSP；影子猎人

### 检索摘要

代表作：种子与银河系空间坐标的换算以达到在银河系上刻字的目的

### 清洗后的结构化资料

代表作：种子与银河系空间坐标的换算以达到在银河系上刻字的目的

### 常见检索问法

- `影子猎人 是谁？`
- `影子猎人 在戴森球计划社区有什么贡献？`
- `影子猎人 有哪些代表作、蓝图、mod 或视频？`

<!-- RAG_CHUNK_END -->

<!-- RAG_CHUNK_START id="dsp-person-思危在澳洲-5ee79e" type="person_profile" -->
## DSP人物档案：思危在澳洲

### 元数据

- chunk_id: `dsp-person-思危在澳洲-5ee79e`
- entity_type: `person_or_community_member`
- name: `思危在澳洲`
- source_file: `DSP-UP/思危在澳洲.md`
- visibility: `public_with_verification`
- answer_policy: 以“社区资料整理/当前资料显示”的口吻回答；涉及争议、版本、数据和个人评价时提示交叉核验。
- aliases_or_ids: Q群ID: 思危在澳洲；B站ID: 思危在澳洲
- tags: 视频作者；争议内容需核验
- keywords: 戴森球计划；DSP；思危在澳洲；视频作者；争议内容需核验

### 检索摘要

视频作者。社区资料提示：其部分视频内容存在较大争议或可能与当前版本、主流机制理解不一致。回答相关问题时，应提醒用户结合游戏版本、数据验证和其他来源交叉核验；同时可说明其视频制作观感较好。

### 清洗后的结构化资料

### 基本信息

| ID | 内容 |
|------|------|
| Q群ID | 思危在澳洲 |
| B站ID | 思危在澳洲 |

### 简介

视频作者。社区资料提示：其部分视频内容存在较大争议或可能与当前版本、主流机制理解不一致。回答相关问题时，应提醒用户结合游戏版本、数据验证和其他来源交叉核验；同时可说明其视频制作观感较好。

### 身份标签

- 视频作者
- 争议内容需核验

### 常见检索问法

- `思危在澳洲 是谁？`
- `思危在澳洲 在戴森球计划社区有什么贡献？`
- `思危在澳洲 有哪些代表作、蓝图、mod 或视频？`

<!-- RAG_CHUNK_END -->

<!-- RAG_CHUNK_START id="dsp-person-我的小马叫丁真-13563a" type="person_profile" -->
## DSP人物档案：我的小马叫丁真

### 元数据

- chunk_id: `dsp-person-我的小马叫丁真-13563a`
- entity_type: `person_or_community_member`
- name: `我的小马叫丁真`
- source_file: `DSP-UP/我的小马叫丁真.md`
- visibility: `public_with_verification`
- answer_policy: 以“社区资料整理/当前资料显示”的口吻回答；涉及争议、版本、数据和个人评价时提示交叉核验。
- aliases_or_ids: Q群ID: 我的小马叫丁真；B站ID: 我的小马叫丁真
- tags: 早期蓝图制作人；早期视频攻略制作者；在垂直带没转正的时期，他就做出了非麻花的垂直带
- keywords: 戴森球计划；DSP；我的小马叫丁真；早期蓝图制作人；早期视频攻略制作者；在垂直带没转正的时期，他就做出了非麻花的垂直带；蓝图；视频作者

### 检索摘要

早期蓝图制作人；早期视频攻略制作者；在垂直带没转正的时期，他就做出了非麻花的垂直带；大部分蓝图已经落后于版本；目前隐退

### 清洗后的结构化资料

| ID | 内容 |
|------|------|
| Q群ID | 我的小马叫丁真 |
| B站ID | 我的小马叫丁真 |

### B站视频作者

### 身份标签
- 早期蓝图制作人
- 早期视频攻略制作者
- 在垂直带没转正的时期，他就做出了非麻花的垂直带

### 补充说明

- 大部分蓝图已经落后于版本
- 目前隐退

### 常见检索问法

- `我的小马叫丁真 是谁？`
- `我的小马叫丁真 在戴森球计划社区有什么贡献？`
- `我的小马叫丁真 有哪些代表作、蓝图、mod 或视频？`

<!-- RAG_CHUNK_END -->

<!-- RAG_CHUNK_START id="dsp-person-摸鱼的slyf-02749c" type="person_profile" -->
## DSP人物档案：摸鱼的slyf

### 元数据

- chunk_id: `dsp-person-摸鱼的slyf-02749c`
- entity_type: `person_or_community_member`
- name: `摸鱼的slyf`
- source_file: `DSP-UP/摸鱼的slyf.md`
- visibility: `public_with_verification`
- answer_policy: 以“社区资料整理/当前资料显示”的口吻回答；涉及争议、版本、数据和个人评价时提示交叉核验。
- aliases_or_ids: Q群ID: 摸鱼的slyf；B站ID: 摸鱼的slyf(存疑)
- tags: 蓝图贡献者；存档测试者；10-30万糖测试存档贡献者；银河系首位10PW贡献者；2023-2024年主要仙术球蓝图贡献者；奇观爱好者；无偏非密铺混带产线蓝图作者
- keywords: 戴森球计划；DSP；摸鱼的slyf；摸鱼的slyf(存疑)；蓝图贡献者；存档测试者；10-30万糖测试存档贡献者；银河系首位10PW贡献者；2023-2024年主要仙术球蓝图贡献者；奇观爱好者；无偏非密铺混带产线蓝图作者；蓝图；密铺；混带；仙术；测试；PW

### 检索摘要

（待补充）；蓝图贡献者；存档测试者；10-30万糖测试存档贡献者；银河系首位10PW贡献者，；2023-2024年主要仙术球蓝图贡献者；奇观爱好者；无偏非密铺混带产线蓝图作者

### 清洗后的结构化资料

### 基本信息

| ID | 内容 |
|------|------|
| Q群ID | 摸鱼的slyf |
| B站ID | 摸鱼的slyf(存疑) |

### B站主页

（待补充）

### 身份标签

- 蓝图贡献者
- 存档测试者
- 10-30万糖测试存档贡献者
- 银河系首位10PW贡献者，
- 2023-2024年主要仙术球蓝图贡献者
- 奇观爱好者
- 无偏非密铺混带产线蓝图作者

### 补充说明

不喜欢被打扰

### 常见检索问法

- `摸鱼的slyf 是谁？`
- `摸鱼的slyf 在戴森球计划社区有什么贡献？`
- `摸鱼的slyf 有哪些代表作、蓝图、mod 或视频？`

<!-- RAG_CHUNK_END -->

<!-- RAG_CHUNK_START id="dsp-person-新星-10ba49" type="person_profile" -->
## DSP人物档案：新星

### 元数据

- chunk_id: `dsp-person-新星-10ba49`
- entity_type: `person_or_community_member`
- name: `新星`
- source_file: `DSP-UP/新星.md`
- visibility: `public_with_verification`
- answer_policy: 以“社区资料整理/当前资料显示”的口吻回答；涉及争议、版本、数据和个人评价时提示交叉核验。
- aliases_or_ids: 未记录
- tags: 未记录
- keywords: 戴森球计划；DSP；新星；蓝图；创世之书

### 检索摘要

蓝图作者；创世之书蓝图作者

### 清洗后的结构化资料

- 蓝图作者
- 创世之书蓝图作者

### 常见检索问法

- `新星 是谁？`
- `新星 在戴森球计划社区有什么贡献？`
- `新星 有哪些代表作、蓝图、mod 或视频？`

<!-- RAG_CHUNK_END -->

<!-- RAG_CHUNK_START id="dsp-person-旧日不在-b60362" type="person_profile" -->
## DSP人物档案：旧日不在

### 元数据

- chunk_id: `dsp-person-旧日不在-b60362`
- entity_type: `person_or_community_member`
- name: `旧日不在`
- source_file: `DSP-UP/旧日不在.md`
- visibility: `public_with_verification`
- answer_policy: 以“社区资料整理/当前资料显示”的口吻回答；涉及争议、版本、数据和个人评价时提示交叉核验。
- aliases_or_ids: 未记录
- tags: 未记录
- keywords: 戴森球计划；DSP；旧日不在；mod；创世之书

### 检索摘要

创世之书mod作者之一

### 清洗后的结构化资料

- 创世之书mod作者之一

### 常见检索问法

- `旧日不在 是谁？`
- `旧日不在 在戴森球计划社区有什么贡献？`
- `旧日不在 有哪些代表作、蓝图、mod 或视频？`

<!-- RAG_CHUNK_END -->

<!-- RAG_CHUNK_START id="dsp-person-是叶语啊-2b75d2" type="person_profile" -->
## DSP人物档案：是叶语啊

### 元数据

- chunk_id: `dsp-person-是叶语啊-2b75d2`
- entity_type: `person_or_community_member`
- name: `是叶语啊`
- source_file: `DSP-UP/是叶语啊.md`
- visibility: `public_with_verification`
- answer_policy: 以“社区资料整理/当前资料显示”的口吻回答；涉及争议、版本、数据和个人评价时提示交叉核验。
- aliases_or_ids: Q群ID: 是叶语啊；B站ID: 是叶语啊；其他称呼: 星辉
- tags: 蓝图制作者
- keywords: 戴森球计划；DSP；是叶语啊；星辉；蓝图制作者；蓝图

### 检索摘要

高质量蓝图制作者。

### 清洗后的结构化资料

### 基本信息

| ID | 内容 |
|------|------|
| Q群ID | 是叶语啊 |
| B站ID | 是叶语啊 |
| 其他称呼 | 星辉 |

### 简介

高质量蓝图制作者。

### 身份标签

- 蓝图制作者

### 蓝图作品

- 超市单片
- 等

### 社群备注

曾在清理不活跃成员时误移除 void，作为社群管理逸事记录。

### 常见检索问法

- `是叶语啊 是谁？`
- `是叶语啊 在戴森球计划社区有什么贡献？`
- `是叶语啊 有哪些代表作、蓝图、mod 或视频？`

<!-- RAG_CHUNK_END -->

<!-- RAG_CHUNK_START id="dsp-person-晨隐_-731d62" type="person_profile" -->
## DSP人物档案：晨隐_

### 元数据

- chunk_id: `dsp-person-晨隐_-731d62`
- entity_type: `person_or_community_member`
- name: `晨隐_`
- source_file: `DSP-UP/晨隐_.md`
- visibility: `public_with_verification`
- answer_policy: 以“社区资料整理/当前资料显示”的口吻回答；涉及争议、版本、数据和个人评价时提示交叉核验。
- aliases_or_ids: Q群ID: 晨隐_；B站ID: 晨隐_
- tags: 工具开发者；编程高手；DSP数字电路奠基人之一
- keywords: 戴森球计划；DSP；晨隐_；工具开发者；编程高手；DSP数字电路奠基人之一；蓝图；工具；数字电路

### 检索摘要

工具开发者

### 清洗后的结构化资料

### 基本信息

| ID | 内容 |
|------|------|
| Q群ID | 晨隐_ |
| B站ID | 晨隐_ |

### 简介

工具开发者

### B站主页
（待补充）

### 身份标签

- 工具开发者
- 编程高手
- DSP数字电路奠基人之一

### 精通

- 数字电路
- 编程

### 代表作

- 晨隐蓝图变换工具 （https://cying.xyz/DSP/editBluePrint/）
- 戴森球图像识别
- 戴森球神经网络存档

### 常见检索问法

- `晨隐_ 是谁？`
- `晨隐_ 在戴森球计划社区有什么贡献？`
- `晨隐_ 有哪些代表作、蓝图、mod 或视频？`

<!-- RAG_CHUNK_END -->

<!-- RAG_CHUNK_START id="dsp-person-机甲海星-965d1d" type="person_profile" -->
## DSP人物档案：机甲海星

### 元数据

- chunk_id: `dsp-person-机甲海星-965d1d`
- entity_type: `person_or_community_member`
- name: `机甲海星`
- source_file: `DSP-UP/机甲海星.md`
- visibility: `public_with_verification`
- answer_policy: 以“社区资料整理/当前资料显示”的口吻回答；涉及争议、版本、数据和个人评价时提示交叉核验。
- aliases_or_ids: Q群ID: 机甲海星；B站ID: 机甲海星；R2ID: starfi5h
- tags: mod作者；编程高手
- keywords: 戴森球计划；DSP；机甲海星；starfi5h；mod作者；编程高手；mod；官方

### 检索摘要

（待补充）

### 清洗后的结构化资料

### 基本信息

| ID | 内容 |
|------|------|
| Q群ID | 机甲海星 |
| B站ID | 机甲海星 |
| R2ID | starfi5h |

### 简介

（待补充）

### 身份标签

- mod作者
- 编程高手

### 精通

- mod制作
- 编程

### mod作品

- bulletTime（速度控制mod）
- 模拟帧（暴力优化mod）
- 全球喷涂（强效作弊mod）
- 统计面板（已被官方吸收）

### 其他代表作

在desynced、炼金工厂等游戏也有不俗的贡献

### 常见检索问法

- `机甲海星 是谁？`
- `机甲海星 在戴森球计划社区有什么贡献？`
- `机甲海星 有哪些代表作、蓝图、mod 或视频？`

<!-- RAG_CHUNK_END -->

<!-- RAG_CHUNK_START id="dsp-person-林凌-6eb87d" type="person_profile" -->
## DSP人物档案：林凌

### 元数据

- chunk_id: `dsp-person-林凌-6eb87d`
- entity_type: `person_or_community_member`
- name: `林凌`
- source_file: `DSP-UP/林凌.md`
- visibility: `public_with_verification`
- answer_policy: 以“社区资料整理/当前资料显示”的口吻回答；涉及争议、版本、数据和个人评价时提示交叉核验。
- aliases_or_ids: Q群ID: 林凌；B站ID: 林凌
- tags: 单基地432养殖奠基人之一
- keywords: 戴森球计划；DSP；林凌；单基地432养殖奠基人之一；蓝图；黑雾

### 检索摘要

蓝图制作人、科研人

### 清洗后的结构化资料

### 基本信息

| ID | 内容 |
|------|------|
| Q群ID | 林凌 |
| B站ID | 林凌 |

### 简介

蓝图制作人、科研人

### 身份标签

- 单基地432养殖奠基人之一

### B站主页

（待补充）

### 精通

- 编程
- 数学

### 蓝图作品

- 火柴人
- 零卡洛斯
- 单基地432养殖奠基人之一

### 其他作品

- 矿物越多矿物越少
- 432养殖

### 补充说明

零卡洛斯指的是0材料、0额外材料的机甲，极度节约前期成本
432养殖指阉割黑雾至3个基地，这样黑雾需要的能量少

### 常见检索问法

- `林凌 是谁？`
- `林凌 在戴森球计划社区有什么贡献？`
- `林凌 有哪些代表作、蓝图、mod 或视频？`

<!-- RAG_CHUNK_END -->

<!-- RAG_CHUNK_START id="dsp-person-橙棂九月-3b9953" type="person_profile" -->
## DSP人物档案：橙棂九月

### 元数据

- chunk_id: `dsp-person-橙棂九月-3b9953`
- entity_type: `person_or_community_member`
- name: `橙棂九月`
- source_file: `DSP-UP/橙棂九月.md`
- visibility: `public_with_verification`
- answer_policy: 以“社区资料整理/当前资料显示”的口吻回答；涉及争议、版本、数据和个人评价时提示交叉核验。
- aliases_or_ids: Q群ID: 橙棂九月；B站ID: 橙棂九月；R2ID: blacksnipebiu
- tags: 初代mod作者
- keywords: 戴森球计划；DSP；橙棂九月；blacksnipebiu；初代mod作者；mod；工具

### 检索摘要

初代知名mod作者

### 清洗后的结构化资料

### 基本信息

| ID | 内容 |
|------|------|
| Q群ID | 橙棂九月 |
| B站ID | 橙棂九月 |
| R2ID | blacksnipebiu |

### 简介

初代知名mod作者

### B站主页

- （待补充）

### 身份标签

- 初代mod作者

### 精通

- mod制作
- 编程

### mod作品

- 戴森球工具箱
- Auxiliaryfunction AUX辅助
- Multifunction_mod OP（强效作弊mod）
- PlanetMiner 星球矿机（强效作弊mod）
- 等

### 常见检索问法

- `橙棂九月 是谁？`
- `橙棂九月 在戴森球计划社区有什么贡献？`
- `橙棂九月 有哪些代表作、蓝图、mod 或视频？`

<!-- RAG_CHUNK_END -->

<!-- RAG_CHUNK_START id="dsp-person-氢碳钾xy-84719e" type="person_profile" -->
## DSP人物档案：氢碳钾xy

### 元数据

- chunk_id: `dsp-person-氢碳钾xy-84719e`
- entity_type: `person_or_community_member`
- name: `氢碳钾xy`
- source_file: `DSP-UP/氢碳钾xy.md`
- visibility: `public_with_verification`
- answer_policy: 以“社区资料整理/当前资料显示”的口吻回答；涉及争议、版本、数据和个人评价时提示交叉核验。
- aliases_or_ids: Q群ID: 氢碳钾xy；B站ID: 氢碳钾xy
- tags: 蓝图制作者
- keywords: 戴森球计划；DSP；氢碳钾xy；蓝图制作者；蓝图；白糖；混带

### 检索摘要

蓝图制作者；（待补充）；混带蓝图；无偏蓝图；1875糖；5100糖；2805-11250分布式白糖；180彩糖；562火箭；57.6K太阳帆；27K增产剂

### 清洗后的结构化资料

### 基本信息

| ID | 内容 |
|------|------|
| Q群ID | 氢碳钾xy |
| B站ID | 氢碳钾xy |

### 身份标签

- 蓝图制作者

### B站主页

- （待补充）

### 精通

- 混带蓝图
- 无偏蓝图

### 蓝图作品

- 1875糖
- 5100糖
- 2805-11250分布式白糖
- 180彩糖
- 562火箭
- 57.6K太阳帆
- 27K增产剂

### 常见检索问法

- `氢碳钾xy 是谁？`
- `氢碳钾xy 在戴森球计划社区有什么贡献？`
- `氢碳钾xy 有哪些代表作、蓝图、mod 或视频？`

<!-- RAG_CHUNK_END -->

<!-- RAG_CHUNK_START id="dsp-person-流浪法师悠米-e39d18" type="person_profile" -->
## DSP人物档案：流浪法师悠米

### 元数据

- chunk_id: `dsp-person-流浪法师悠米-e39d18`
- entity_type: `person_or_community_member`
- name: `流浪法师悠米`
- source_file: `DSP-UP/流浪法师悠米.md`
- visibility: `public_with_verification`
- answer_policy: 以“社区资料整理/当前资料显示”的口吻回答；涉及争议、版本、数据和个人评价时提示交叉核验。
- aliases_or_ids: Q群ID: 流浪法师悠米；B站ID: 流浪法师悠米；R2ID: cat_yummi；其他称呼: ChatCAT
- tags: 视频作者；攻略作者；邪道速通者；整活蓝图制作者；仙术蓝图作者；仙术原理探究者；mod作者；PW级爱好者
- keywords: 戴森球计划；DSP；流浪法师悠米；cat_yummi；ChatCAT；视频作者；攻略作者；邪道速通者；整活蓝图制作者；仙术蓝图作者；仙术原理探究者；mod作者；PW级爱好者；蓝图；mod；速通；混带；仙术；工具；五周年点亮计划；PW
- bv_ids: BV1HJ4m1M7Fo；BV1ibiweEE9y；BV17JxeeEEmN；BV199B4YKEpn；BV1BEQkYHECb；BV1TvdkYLEkd；BV1rDNdzWEvC；BV1MVZRBLEzV；BV1HdWdejEtn；BV1saTXzoEzd；BV1uNrsBHE6j

### 检索摘要

攻略视频作者

### 清洗后的结构化资料

### 基本信息

| ID | 内容 |
|------|------|
| Q群ID | 流浪法师悠米 |
| B站ID | 流浪法师悠米 |
| R2ID | cat_yummi |
| 其他称呼 | ChatCAT |

### 简介

攻略视频作者

### B站主页

https://space.bilibili.com/394761773

### 身份标签

- 视频作者
- 攻略作者
- 邪道速通者
- 整活蓝图制作者
- 仙术蓝图作者
- 仙术原理探究者
- mod作者
- PW级爱好者

### 科普系列视频

- 流速扫盲 BV1HJ4m1M7Fo
- 增产剂的作用扫盲 BV1ibiweEE9y
- 戴森壳扫盲 BV17JxeeEEmN
- 2024年末战斗总结 BV199B4YKEpn
- 逻辑帧分析 BV1BEQkYHECb
- 混带的3种结构 BV1TvdkYLEkd
- 光子前后思路解析 BV1rDNdzWEvC
- 不堵氢计划 BV1MVZRBLEzV
- 一分钟科普 BV1HdWdejEtn

### 流程系列视频

- 最少建筑手搓过关 BV1saTXzoEzd
- 27分10秒速通戴森球 BV1uNrsBHE6j

### 其他代表作

- 毕加索机甲
- 432奠基人之一
- 五周年点亮计划摸鱼者

### 补充说明

蓝图代表作，仙术代表作、工具代表作均不列举。
因为过于暴力，猫夫人让猫不要发

### 常见检索问法

- `流浪法师悠米 是谁？`
- `流浪法师悠米 在戴森球计划社区有什么贡献？`
- `流浪法师悠米 有哪些代表作、蓝图、mod 或视频？`

<!-- RAG_CHUNK_END -->

<!-- RAG_CHUNK_START id="dsp-person-看客之眼-0a7654" type="person_profile" -->
## DSP人物档案：看客之眼

### 元数据

- chunk_id: `dsp-person-看客之眼-0a7654`
- entity_type: `person_or_community_member`
- name: `看客之眼`
- source_file: `DSP-UP/看客之眼.md`
- visibility: `public_with_verification`
- answer_policy: 以“社区资料整理/当前资料显示”的口吻回答；涉及争议、版本、数据和个人评价时提示交叉核验。
- aliases_or_ids: 未记录
- tags: 未记录
- keywords: 戴森球计划；DSP；看客之眼

### 检索摘要

参与过CIDT，其余情况不明。

### 清洗后的结构化资料

参与过CIDT，其余情况不明。

### 常见检索问法

- `看客之眼 是谁？`
- `看客之眼 在戴森球计划社区有什么贡献？`
- `看客之眼 有哪些代表作、蓝图、mod 或视频？`

<!-- RAG_CHUNK_END -->

<!-- RAG_CHUNK_START id="dsp-person-莳槡_makuwa-abc6ee" type="person_profile" -->
## DSP人物档案：莳槡_makuwa

### 元数据

- chunk_id: `dsp-person-莳槡_makuwa-abc6ee`
- entity_type: `person_or_community_member`
- name: `莳槡_makuwa`
- source_file: `DSP-UP/莳槡_makuwa.md`
- visibility: `public_with_verification`
- answer_policy: 以“社区资料整理/当前资料显示”的口吻回答；涉及争议、版本、数据和个人评价时提示交叉核验。
- aliases_or_ids: Q群ID: 莳槡_makuwa；B站ID: 莳槡_makuwa；R2ID: shisang_makuwa1；其他称呼: 叶天帝
- tags: 满格六边形战士；低卡顿混带原理奠基人；密铺奠基人；模组开发者；视频作者；密铺教程视频作者
- keywords: 戴森球计划；DSP；莳槡_makuwa；shisang_makuwa1；叶天帝；满格六边形战士；低卡顿混带原理奠基人；密铺奠基人；模组开发者；视频作者；密铺教程视频作者；mod；模组；速通；白糖；密铺；混带；官方；计算器
- bv_ids: BV1w3411S7AH；BV19R4y1z7Jc

### 检索摘要

满格六边形战士，低卡顿混带原理奠基人之一，密铺奠基人之一

### 清洗后的结构化资料

### 基本信息

| ID | 内容 |
|------|------|
| Q群ID | 莳槡_makuwa |
| B站ID | 莳槡_makuwa |
| R2ID | shisang_makuwa1 |
| 其他称呼 | 叶天帝 |

### 简介

满格六边形战士，低卡顿混带原理奠基人之一，密铺奠基人之一

### B站主页

https://space.bilibili.com/16051534

### 精通

- 似乎没有不擅长的

### 身份标签

- 满格六边形战士
- 低卡顿混带原理奠基人
- 密铺奠基人
- 模组开发者
- 视频作者
- 密铺教程视频作者

### 系列视频

- BV1w3411S7AH 密铺教程
- BV19R4y1z7Jc 游戏机制

### mod作品
- LongerBelts
- 并带不满修复mod（现已被官方吸收）

### 其他代表作

- 配平计算器网站 https://dsp-calc.pro/
- 密铺教程视频
- 2小时内速通的可能性讨论
- 戴森球数值统计excel

- 全球六万白糖的走线参与者

### 补充说明

其中并带不满修复mod已被官方吸收融入游戏中

### 常见检索问法

- `莳槡_makuwa 是谁？`
- `莳槡_makuwa 在戴森球计划社区有什么贡献？`
- `莳槡_makuwa 有哪些代表作、蓝图、mod 或视频？`

<!-- RAG_CHUNK_END -->

<!-- RAG_CHUNK_START id="dsp-person-萌泪酱最可爱啦-43cbdc" type="person_profile" -->
## DSP人物档案：萌泪酱最可爱啦

### 元数据

- chunk_id: `dsp-person-萌泪酱最可爱啦-43cbdc`
- entity_type: `person_or_community_member`
- name: `萌泪酱最可爱啦`
- source_file: `DSP-UP/萌泪酱最可爱啦.md`
- visibility: `public_with_verification`
- answer_policy: 以“社区资料整理/当前资料显示”的口吻回答；涉及争议、版本、数据和个人评价时提示交叉核验。
- aliases_or_ids: 未记录
- tags: 未记录
- keywords: 戴森球计划；DSP；萌泪酱最可爱啦；mod

### 检索摘要

万物分馏mod作者

### 清洗后的结构化资料

- 万物分馏mod作者

### 常见检索问法

- `萌泪酱最可爱啦 是谁？`
- `萌泪酱最可爱啦 在戴森球计划社区有什么贡献？`
- `萌泪酱最可爱啦 有哪些代表作、蓝图、mod 或视频？`

<!-- RAG_CHUNK_END -->

<!-- RAG_CHUNK_START id="dsp-person-虚幻道长-07e5b8" type="person_profile" -->
## DSP人物档案：虚幻道长

### 元数据

- chunk_id: `dsp-person-虚幻道长-07e5b8`
- entity_type: `person_or_community_member`
- name: `虚幻道长`
- source_file: `DSP-UP/虚幻道长.md`
- visibility: `public_with_verification`
- answer_policy: 以“社区资料整理/当前资料显示”的口吻回答；涉及争议、版本、数据和个人评价时提示交叉核验。
- aliases_or_ids: Q群ID: 虚幻道长；B站ID: 虚幻道长；其他称呼: 坚果墙、小程
- tags: dsp-bwiki 编辑者；争议内容需核验
- keywords: 戴森球计划；DSP；虚幻道长；坚果墙、小程；dsp-bwiki 编辑者；争议内容需核验；黑雾；计算器

### 检索摘要

dsp-bwiki 编辑者。社区资料提示：其部分攻略、模板或计算内容存在争议，可能过时或需要结合版本重新验证。回答相关问题时，应提醒用户谨慎分辨、交叉核验，不应把单一资料源作为最终结论。

### 清洗后的结构化资料

### 基本信息

| ID | 内容 |
|------|------|
| Q群ID | 虚幻道长 |
| B站ID | 虚幻道长 |
| 其他称呼 | 坚果墙、小程 |

### 简介

dsp-bwiki 编辑者。社区资料提示：其部分攻略、模板或计算内容存在争议，可能过时或需要结合版本重新验证。回答相关问题时，应提醒用户谨慎分辨、交叉核验，不应把单一资料源作为最终结论。

### 身份标签

- dsp-bwiki 编辑者
- 争议内容需核验

### 代表作品

- 黑雾掉落超市（争议）
- 蓝红糖产线图（可能过时）
- 原油处理（争议）
- 60基站分拣（争议）
- 44串联分馏塔（争议）
- bwiki戴森壳计算器
- bwiki网页模板

### 补充说明

经常出没于 Q 群、B站、百度贴吧、小黑盒等社区平台。

### 常见检索问法

- `虚幻道长 是谁？`
- `虚幻道长 在戴森球计划社区有什么贡献？`
- `虚幻道长 有哪些代表作、蓝图、mod 或视频？`

<!-- RAG_CHUNK_END -->

<!-- RAG_CHUNK_START id="dsp-person-重装小兔-edcc04" type="person_profile" -->
## DSP人物档案：重装小兔

### 元数据

- chunk_id: `dsp-person-重装小兔-edcc04`
- entity_type: `person_or_community_member`
- name: `重装小兔`
- source_file: `DSP-UP/重装小兔.md`
- visibility: `public_with_verification`
- answer_policy: 以“社区资料整理/当前资料显示”的口吻回答；涉及争议、版本、数据和个人评价时提示交叉核验。
- aliases_or_ids: Q群ID: 重装小兔；B站ID: 重装小兔
- tags: 视频攻略作者；蓝图制作人；白糖单推人
- keywords: 戴森球计划；DSP；重装小兔；视频攻略作者；蓝图制作人；白糖单推人；蓝图；白糖

### 检索摘要

视频攻略作者、蓝图制作人、白糖单推人、历代单片白糖主力之一。

### 清洗后的结构化资料

### 基本信息

| ID | 内容 |
|------|------|
| Q群ID | 重装小兔 |
| B站ID | 重装小兔 |

### 简介

视频攻略作者、蓝图制作人、白糖单推人、历代单片白糖主力之一。

### 身份标签

- 视频攻略作者
- 蓝图制作人
- 白糖单推人

### 代表作

- 全球6万白糖作者之一
- 重装小兔825极地锅

### 补充说明

- 目前几乎隐退

### 常见检索问法

- `重装小兔 是谁？`
- `重装小兔 在戴森球计划社区有什么贡献？`
- `重装小兔 有哪些代表作、蓝图、mod 或视频？`

<!-- RAG_CHUNK_END -->

<!-- RAG_CHUNK_START id="dsp-person-钱佬-e98716" type="person_profile" -->
## DSP人物档案：钱佬

### 元数据

- chunk_id: `dsp-person-钱佬-e98716`
- entity_type: `person_or_community_member`
- name: `钱佬`
- source_file: `DSP-UP/钱佬.md`
- visibility: `public_with_verification`
- answer_policy: 以“社区资料整理/当前资料显示”的口吻回答；涉及争议、版本、数据和个人评价时提示交叉核验。
- aliases_or_ids: 未记录
- tags: 未记录
- keywords: 戴森球计划；DSP；钱佬；蓝图；创世之书

### 检索摘要

创世之书蓝图作者

### 清洗后的结构化资料

- 创世之书蓝图作者

### 常见检索问法

- `钱佬 是谁？`
- `钱佬 在戴森球计划社区有什么贡献？`
- `钱佬 有哪些代表作、蓝图、mod 或视频？`

<!-- RAG_CHUNK_END -->

<!-- RAG_CHUNK_START id="dsp-person-阿七寇大先生-d923e6" type="person_profile" -->
## DSP人物档案：阿七寇大先生

### 元数据

- chunk_id: `dsp-person-阿七寇大先生-d923e6`
- entity_type: `person_or_community_member`
- name: `阿七寇大先生`
- source_file: `DSP-UP/阿七寇大先生.md`
- visibility: `public_with_verification`
- answer_policy: 以“社区资料整理/当前资料显示”的口吻回答；涉及争议、版本、数据和个人评价时提示交叉核验。
- aliases_or_ids: Q群ID: 阿七寇大先生；B站ID: 阿七寇大先生；R2ID: Mr_AqiKouda
- tags: 蓝图制作者；编程高手
- keywords: 戴森球计划；DSP；阿七寇大先生；Mr_AqiKouda；蓝图制作者；编程高手；蓝图；数字电路

### 检索摘要

DSP数字电路奠基人之一

### 清洗后的结构化资料

### 基本信息

| ID | 内容 |
|------|------|
| Q群ID | 阿七寇大先生 |
| B站ID | 阿七寇大先生 |
| R2ID | Mr_AqiKouda |

### 简介

DSP数字电路奠基人之一

### B站主页
（待补充）

### 身份标签

- 蓝图制作者
- 编程高手

### 精通

- 数字电路
- 编程

### 代表作

- 猜拳机
- 花瓶机甲蓝图
- 原神播放器

### 常见检索问法

- `阿七寇大先生 是谁？`
- `阿七寇大先生 在戴森球计划社区有什么贡献？`
- `阿七寇大先生 有哪些代表作、蓝图、mod 或视频？`

<!-- RAG_CHUNK_END -->

<!-- RAG_CHUNK_START id="dsp-person-难辞旧安-f6929f" type="person_profile" -->
## DSP人物档案：难辞旧安

### 元数据

- chunk_id: `dsp-person-难辞旧安-f6929f`
- entity_type: `person_or_community_member`
- name: `难辞旧安`
- source_file: `DSP-UP/难辞旧安.md`
- visibility: `public_with_verification`
- answer_policy: 以“社区资料整理/当前资料显示”的口吻回答；涉及争议、版本、数据和个人评价时提示交叉核验。
- aliases_or_ids: Q群ID: 难辞旧安；B站ID: 难辞旧安；B站ID: 都是渣渣
- tags: 蓝图制作者；单片蓝图制作高手；PW级爱好者；银河系寡头；五周年点亮计划发起人之一
- keywords: 戴森球计划；DSP；难辞旧安；都是渣渣；蓝图制作者；单片蓝图制作高手；PW级爱好者；银河系寡头；五周年点亮计划发起人之一；蓝图；白糖；五周年点亮计划；PW

### 检索摘要

单片蓝图制作高手

### 清洗后的结构化资料

### 基本信息

| ID | 内容 |
|------|------|
| Q群ID | 难辞旧安 |
| B站ID | 难辞旧安 |
| B站ID | 都是渣渣 |

### 简介

单片蓝图制作高手

### B站主页

- （待补充）

### 身份标签

- 蓝图制作者
- 单片蓝图制作高手
- PW级爱好者
- 银河系寡头
- 五周年点亮计划发起人之一

### 蓝图作品

- 4500透镜
- 3000白糖
- 400黄棒
- 960小火箭
- 72k太阳帆
- 86.4k太阳帆
- 16875增产剂

### 常见检索问法

- `难辞旧安 是谁？`
- `难辞旧安 在戴森球计划社区有什么贡献？`
- `难辞旧安 有哪些代表作、蓝图、mod 或视频？`

<!-- RAG_CHUNK_END -->

<!-- RAG_CHUNK_START id="dsp-person-鱼叉-a6b28c" type="person_profile" -->
## DSP人物档案：鱼叉

### 元数据

- chunk_id: `dsp-person-鱼叉-a6b28c`
- entity_type: `person_or_community_member`
- name: `鱼叉`
- source_file: `DSP-UP/鱼叉.md`
- visibility: `public_with_verification`
- answer_policy: 以“社区资料整理/当前资料显示”的口吻回答；涉及争议、版本、数据和个人评价时提示交叉核验。
- aliases_or_ids: Q群ID: 鱼叉；B站ID: aborner
- tags: 蓝图制作者；机制研究员；速通爱好者
- keywords: 戴森球计划；DSP；鱼叉；aborner；蓝图制作者；机制研究员；速通爱好者；蓝图；速通

### 检索摘要

蓝图制作者、机制研究员、速通爱好者

### 清洗后的结构化资料

### 基本信息

| ID | 内容 |
|------|------|
| Q群ID | 鱼叉 |
| B站ID | aborner |

### 简介

蓝图制作者、机制研究员、速通爱好者

### B站主页

（待补充）

### 身份标签

- 蓝图制作者
- 机制研究员
- 速通爱好者

### 蓝图代表作

- 单基地1080科学养殖

### 视频代表作

- 17小时万糖

### 常见检索问法

- `鱼叉 是谁？`
- `鱼叉 在戴森球计划社区有什么贡献？`
- `鱼叉 有哪些代表作、蓝图、mod 或视频？`

<!-- RAG_CHUNK_END -->
