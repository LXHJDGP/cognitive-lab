# 认知实验室（Cognitive Lab）

**个人认知练习与记录工具**

认知实验室是一个面向成年学习者的个人认知训练小工具，主要围绕工作记忆、连续信息加工、数学推导、逻辑推理和注意控制设计练习。

项目的设计起点是一些具体的认知任务：在多步骤运算中保持中间结果，在复杂论证中维持前提与推理关系，在连续加工中及时更新信息，以及在任务中断后恢复原有思路。

工具参考认知心理学与教育心理学中的相关研究，将部分经典实验范式和教学方法改编为可重复进行的日常练习，并提供题目反馈、难度调整、训练记录和数据导出功能。

**核心内容：** 工作记忆更新、操作广度、渐隐式数学推导、连续推理、单任务注意与中断恢复。

---

## 一、设计思路

工作记忆（Working Memory）是认知活动中的重要组成部分，涉及信息的暂时保持与操作。在数学运算、语言理解、问题解决和逻辑推理等任务中，个体往往需要同时保持若干信息，并根据当前任务不断更新和使用这些信息。

不同任务对认知加工的要求有所区别。例如：

- 多步骤数学运算需要保持中间结果，并连续执行符号操作；
- 复杂论证需要记住前提，并维持前提与结论之间的关系；
- 双任务活动要求在执行加工任务的同时保持另一组信息；
- 任务中断后的恢复需要重新确认当前目标、任务进度和后续步骤。

这些活动涉及工作记忆、注意控制、知识熟练度和认知策略等多个方面。

本工具据此设置五类练习。各模块具有不同的训练目标，不将它们简单归结为同一种工作记忆训练。

## 二、训练模块

### 1. 工作记忆更新（Working Memory Updating）

**训练目标：** 练习在连续信息输入过程中保持当前信息，并根据新信息及时更新已有内容。

工作记忆更新是工作记忆研究中的重要领域。人在进行连续计算、追踪信息变化或处理动态问题时，都需要不断调整当前保持的信息。

本模块采用两种经典实验范式。

**N-back**

连续呈现字母，判断当前字母是否与前面第 N 个位置的字母相同。

- 1-back：与前一个字母比较。
- 2-back：与前两个字母比较。
- 3-back：与前三个字母比较。

随着 N 值增加，需要监控和更新的信息关系更加复杂。

**Running Memory Span（滚动记忆广度）**

连续呈现一组长度不固定的字母或数字，最后要求回忆最近的若干项，并保持原有顺序。

例如：

`A — C — D — B — F — E — G`

如果要求回忆最后四项，答案为：

`B — F — E — G`

**练习方式：**

从低难度开始，逐渐增加 N 值、序列长度或信息更新频率。优先保证准确率，再增加任务复杂度。

**记录指标：**

- 正确识别率；
- 漏答与误答次数；
- 序列回忆准确率；
- 不同难度下的表现变化。

**研究依据：**

- Kirchner, W. K. (1958). *Age Differences in Short-Term Retention of Rapidly Changing Information*. Journal of Experimental Psychology, 55(4), 352–358.
- Pollack, I., Johnson, L. B., & Knaff, P. R. (1959). *Running Memory Span*. Journal of Experimental Psychology, 57(3), 137–146.

这两种任务均有较长的实验研究历史。本工具采用的是适合个人练习的简化版本。

### 2. 操作广度（Operation Span）

**训练目标：** 练习在执行信息加工任务的同时，保持另一组信息。

复杂跨度任务（Complex Span Tasks）是工作记忆研究中常见的实验范式。它与单纯记忆数字不同，要求参与者同时承担加工和保持两类任务。

本模块采用 Operation Span 的基本结构。

**任务示例：**

| 数学判断 | 需要记住的字母 |
|---|---|
| 3 + 4 = 7（正确） | K |
| 6 × 2 = 10（错误） | M |
| 8 − 3 = 5（正确） | R |

完成全部判断后，按照原有顺序回忆：

`K — M — R`

**练习方式：**

1. 判断数学表达式的正确性。
2. 记住随后出现的字母。
3. 重复上述过程。
4. 在序列结束后按顺序回忆字母。

初期从较短的序列开始，逐渐增加记忆项目数量。

**记录指标：**

- 数学判断正确率；
- 字母回忆正确率；
- 顺序错误；
- 不同序列长度下的表现。

两项任务分别记录，避免只关注记忆结果而忽略加工任务本身。

**研究依据：**

Unsworth, N., Heitz, R. P., Schrock, J. C., & Engle, R. W. (2005). *An Automated Version of the Operation Span Task*. Behavior Research Methods, 37, 498–505.

https://doi.org/10.3758/BF03192720

### 3. 渐隐式数学推导（Faded Worked Examples）

**训练目标：** 练习数学程序知识，逐步减少对解题提示的依赖，提高基础操作的熟练程度。

数学问题解决不仅涉及概念理解，还涉及运算程序、符号变换和连续步骤的执行。

当基础操作尚不熟练时，学习者需要投入较多认知资源处理每一步操作，可能增加复杂问题的加工负担。

渐隐式例题（Faded Worked Examples）通过逐步撤去解题提示，使学习者从观察完整示范过渡到独立解题。

**训练分为四个阶段：**

| 阶段 | 练习形式 |
|---|---|
| 完整示范 | 阅读完整解题过程，理解每一步的依据 |
| 补全最后一步 | 根据已有过程独立完成最后一步 |
| 补全多个步骤 | 逐渐减少提示，独立完成连续推导 |
| 独立解题 | 完成一道结构相似的新题 |

例如：

\[
2x+3=11
\]

完整示范：

\[
2x=11-3=8
\]

\[
x=8/2=4
\]

随后逐步隐藏解题步骤，最终要求独立完成同类问题。

**练习内容：**

- 基础运算；
- 代数表达式；
- 方程与不等式；
- 函数关系；
- 数列；
- 概率与基础数学问题。

**记录指标：**

- 补全步骤正确率；
- 独立解题正确率；
- 完成时间；
- 运算错误与步骤遗漏；
- 对相似新题的迁移表现。

**研究依据：**

Renkl, A., Atkinson, R. K., Maier, U. H., & Staley, R. (2002). *From Example Study to Problem Solving: Smooth Transitions Help Learning*. The Journal of Experimental Education, 70(4), 293–315.

https://freidok.uni-freiburg.de/data/47068

该方法主要具有数学教学与学习科学方面的研究依据，不能直接等同于工作记忆容量训练。

### 4. 连续推理（Reasoning Chain）

**训练目标：** 练习在多前提条件下维持推理过程，正确应用推理规则，并形成完整的结论。

本模块主要采用形式逻辑中的演绎推理任务。

**任务示例：**

- 前提一：所有 A 都是 B。
- 前提二：所有 B 都是 C。
- 前提三：D 是 A。

要求逐步推导：

\[
D\in A
\]

\[
D\in B
\]

\[
D\in C
\]

除了最终结论，还需要保留中间推理步骤及其依据。

**练习内容：**

- 三段论；
- 条件推理；
- 关系推理；
- 否定与排除；
- 多前提推理；
- 多层次中间结论推导。

**练习方式：**

从两步推理开始，逐渐增加前提数量和推理长度。完成后检查每一步是否有相应前提支持，是否存在条件遗漏或规则误用。

**记录指标：**

- 前提识别准确率；
- 推理规则使用正确率；
- 中间步骤遗漏；
- 最终结论有效性；
- 无效推导次数。

本模块属于形式推理练习，主要关注逻辑规则的掌握和连续推理表现。

### 5. 单任务注意与中断恢复（Single-task Attention）

**训练目标：** 练习维持当前任务目标，并在任务中断后恢复原有工作状态。

本模块不以完全排除其他想法为目标，而是通过设定明确的任务目标、记录中断情况和制定恢复计划，练习任务管理与注意调节。

**基本练习流程：**

1. 选择一项具体任务，例如阅读一段原著或完成一道数学题。
2. 设定连续工作时段。
3. 记录训练过程中的非计划中断。
4. 如果发生中断，记录当前任务状态。
5. 写下返回任务后的第一步。
6. 重新进入任务并记录恢复情况。

可以使用以下记录表：

| 项目 | 记录内容 |
|---|---|
| 当前任务 | 正在完成什么 |
| 已完成内容 | 当前进度 |
| 中断位置 | 中断前正在处理的环节 |
| 恢复行动 | 返回后首先执行什么 |
| 恢复耗时 | 重新进入任务所需时间 |

例如：

> 当前任务：阅读哲学原著中的一段论证。  
> 已完成：梳理前两个前提。  
> 当前状态：正在分析第三个前提与结论的关系。  
> 下一步：回到原文，检查第三个前提是否能够支持结论。

**记录指标：**

- 目标完成程度；
- 非计划中断次数；
- 中断持续时间；
- 任务恢复时间；
- 恢复后的第一项操作。

**研究依据：**

Leroy, S., & Glomb, T. M. (2018). *Tasks Interrupted: How Anticipating Time Pressure on Resumption of an Interrupted Task Causes Attention Residue and Low Performance on Interrupting Tasks and How a “Ready-to-Resume” Plan Mitigates the Effects*. Organization Science, 29(3), 380–397.

https://doi.org/10.1287/orsc.2017.1184

---

## 三、日常练习安排

建议采用每周五练的方式，每次约15—25分钟。每日安排两项专项练习，并结合一段实际的单任务活动。

| 星期 | 训练内容 | 建议时长 |
|---|---|---:|
| 周一 | 工作记忆更新＋数学操作 | 20分钟 |
| 周二 | 操作广度＋连续推理 | 20分钟 |
| 周三 | 渐隐式数学推导 | 20分钟 |
| 周四 | 工作记忆更新＋单任务注意 | 20分钟 |
| 周五 | 综合练习＋阶段复盘 | 25分钟 |
| 周末 | 休息或自主阅读、数学练习 | 自选 |

上述安排是便于长期坚持的练习建议，并非经过剂量比较研究确定的最优方案。

### 难度调整

系统根据近期同类任务的表现提供难度调整建议，同时允许手动选择题目。

主要调整因素包括：

- N-back 的 N 值；
- 信息序列长度；
- 同时加工的信息数量；
- 数学推导步骤；
- 推理前提数量；
- 任务时间限制。

建议一次主要调整一个难度因素，并在相同难度下积累一定数量的练习记录，再进行比较。

---

## 四、训练记录与表现观察

每次练习结束后，系统记录任务表现，以便观察不同模块的变化。

| 指标 | 记录内容 |
|---|---|
| 正确率 | 正确完成的项目比例 |
| 完成时间 | 完成任务所用时间 |
| 漏答次数 | 未作出有效回答的项目 |
| 错误类型 | 识别、保持、运算、推理等环节的错误 |
| 步骤遗漏 | 未完成规定的中间步骤 |
| 主观用力程度 | 对任务困难程度的自我评价 |
| 中断次数 | 训练过程中的非计划切换 |
| 恢复时间 | 中断后重新进入任务所需的时间 |

建议重点观察同一模块、相近难度下的正确率和完成时间，结合错误类型判断表现变化。

例如：

- N-back 正确率是否随着练习逐渐提高；
- 操作广度任务中，记忆正确率与加工正确率是否出现不同变化；
- 数学推导中，是否减少了基础操作错误；
- 连续推理中，是否减少了前提遗漏；
- 任务中断后，是否能够更快恢复原有工作状态。

系统提供历史记录和趋势统计，支持按训练模块查看个人表现。

### 关于训练迁移

认知训练研究通常区分三种效果：

- **训练效果：** 已经练习过的任务表现提高。
- **近迁移：** 未直接练习、但认知要求相近的任务出现改善。
- **远迁移：** 改善扩展到其他认知领域，例如一般智力、阅读理解或数学学业表现。

现有研究对工作记忆训练的远迁移效果仍存在争议。因此，本工具主要用于记录具体练习的表现变化，并通过新题观察近迁移情况。

---

## 五、相关研究

本工具所采用的方法具有不同的研究来源，需要分别理解。

| 模块 | 主要研究领域 | 相关研究内容 |
|---|---|---|
| 工作记忆更新 | 实验心理学 | 信息更新与短时保持 |
| 操作广度 | 工作记忆研究 | 信息加工与保持的协调 |
| 渐隐式数学推导 | 教育心理学 | 例题学习与独立解题 |
| 连续推理 | 逻辑学、推理心理学 | 演绎规则与推理表现 |
| 单任务注意 | 注意研究、组织行为研究 | 任务中断与恢复计划 |

### 工作记忆训练的迁移问题

Melby-Lervåg、Redick 与 Hulme（2016）对87篇研究、145组实验比较进行了元分析。研究发现，工作记忆训练能够改善部分相似任务的表现，但对于智力、阅读理解和算术等远迁移结果，尚缺乏充分可靠的证据。

Fu 等人（2026）发表的系统综述与元分析纳入55项研究、3492名参与者，发现工作记忆更新训练向记忆跨度任务存在小幅迁移效应。不同训练范式之间的迁移表现并不完全一致。

因此，本工具将工作记忆实验任务、数学教学练习、逻辑推理和注意控制策略分别设置为独立模块，不将它们的训练成绩合并解释为某种总体认知能力。

**参考研究：**

1. Baddeley, A. (2012). Working Memory: Theories, Models, and Controversies. *Annual Review of Psychology*, 63, 1–29.  
   https://doi.org/10.1146/annurev-psych-120710-100422

2. Cowan, N. (2010). The Magical Mystery Four: How Is Working Memory Capacity Limited, and Why? *Current Directions in Psychological Science*, 19(1), 51–57.  
   https://doi.org/10.1177/0963721409359277

3. Raghubar, K. P., Barnes, M. A., & Hecht, S. A. (2010). Working Memory and Mathematics: A Review of Developmental, Individual Difference, and Cognitive Approaches. *Learning and Individual Differences*, 20(2), 110–122.  
   https://doi.org/10.1016/j.lindif.2009.10.005

4. Kirchner, W. K. (1958). Age Differences in Short-Term Retention of Rapidly Changing Information. *Journal of Experimental Psychology*, 55(4), 352–358.  
   https://pubmed.ncbi.nlm.nih.gov/13539317/

5. Pollack, I., Johnson, L. B., & Knaff, P. R. (1959). Running Memory Span. *Journal of Experimental Psychology*, 57(3), 137–146.  
   https://pubmed.ncbi.nlm.nih.gov/13641585/

6. Unsworth, N., Heitz, R. P., Schrock, J. C., & Engle, R. W. (2005). An Automated Version of the Operation Span Task. *Behavior Research Methods*, 37, 498–505.  
   https://doi.org/10.3758/BF03192720

7. Renkl, A., Atkinson, R. K., Maier, U. H., & Staley, R. (2002). From Example Study to Problem Solving: Smooth Transitions Help Learning. *The Journal of Experimental Education*, 70(4), 293–315.  
   https://freidok.uni-freiburg.de/data/47068

8. Leroy, S., & Glomb, T. M. (2018). Tasks Interrupted: How Anticipating Time Pressure on Resumption of an Interrupted Task Causes Attention Residue and Low Performance on Interrupting Tasks and How a “Ready-to-Resume” Plan Mitigates the Effects. *Organization Science*, 29(3), 380–397.  
   https://doi.org/10.1287/orsc.2017.1184

9. Melby-Lervåg, M., Redick, T. S., & Hulme, C. (2016). Working Memory Training Does Not Improve Performance on Measures of Intelligence or Other Measures of “Far Transfer”. *Perspectives on Psychological Science*, 11(4), 512–534.  
   https://pmc.ncbi.nlm.nih.gov/articles/PMC4968033/

10. Fu, J., et al. (2026). The Asymmetry of Working Memory Training Transfer: A Systematic Review and Meta-Analysis. *Psychonomic Bulletin & Review*, 33.  
    https://doi.org/10.3758/s13423-026-02994-5

---

## 六、Windows 使用方法

本工具支持通过本地 HTML 文件运行，无需安装额外的开发环境。

### 下载离线版

1. 在在线工作台右上角点击「下载离线版」。
2. 下载 `认知实验室.html`。
3. 将文件保存到固定文件夹。
4. 使用 Microsoft Edge、Google Chrome 或 Brave 打开。

### 从 GitHub 获取

[GitHub 项目仓库](https://github.com/LXHJDGP/cognitive-lab)

[下载项目 ZIP](https://github.com/LXHJDGP/cognitive-lab/archive/refs/heads/main.zip)

解压后打开 `index.html`。

### 开始使用

1. 进入「今日工作台」查看当天练习安排。
2. 进入相应训练模块，完成练习。
3. 查看逐题解析与结果反馈。
4. 记录主观用力程度及需要注意的步骤。
5. 保存本次训练记录。

---

## 七、记录备份

训练历史保存在浏览器本地存储中。

建议固定使用同一浏览器，并定期导出备份。

| 格式 | 用途 |
|---|---|
| JSON | 完整训练记录的导出与恢复 |
| CSV | 使用 Excel 查看和整理逐次训练数据 |

在在线工作台与离线版本之间迁移记录时，先从原版本导出 JSON，再在目标版本中导入。

本地存储并非加密存储。训练备份可能包含个人备注，请妥善保管，不宜上传至公开仓库。

---

**项目名称：** 认知实验室（Cognitive Lab）  
**项目类型：** 个人认知练习工具  
**运行环境：** Windows / Chromium 系浏览器  
**主要内容：** 工作记忆、数学推导、连续推理与注意控制  
**研究参考：** 认知心理学、数学认知研究、教育心理学与注意控制研究
