# 🎬 Movie Camera Director (电影级影视与漫剧运镜导演)

[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](LICENSE)
[![Skill: Antigravity / Claude / Codex](https://img.shields.io/badge/Agent%20Skill-Antigravity%20%7C%20Claude%20%7C%20Codex-brightgreen)](SKILL.md)
[![AI Video Ready](https://img.shields.io/badge/AI%20Video-Minimax%20H3%20%7C%20Kling%20%7C%20Seedance%20%7C%20Runway-orange)](SKILL.md)

> **专业级影视与漫剧（动态漫画）运镜导演智能体技能。**  
> 将编剧或创作者平淡、初级的分镜描述，重构为具有强烈视觉冲击力、精确几何透视、空间层次感与情绪压迫力的电影级动态分镜，并输出可直接驱动主流 AI 视频生成模型的高权重专业提示词。

---

## 🌟 核心理念与防崩铁律 (Core Philosophy)

漫剧（Motion Comics）与传统纯 3D CG 电影最大的物理区别在于：**底图多为 2D 概念原画或 2.5D 分层插画**。直接套用真人电影运镜极易导致人脸崩坏、肢体畸变或画风撕裂。

`movie-camera-director` 建立了一整套科学严密的**漫剧防崩坏铁律与视效语法**：

1. **反低幼化（严禁初级笼统词）**：严禁使用“镜头拉近”、“镜头推远”、“全景”、“特写”。必须精确指定机位坐标、焦段、物理轨迹与速度曲线。
2. **2D 底图严禁 360° 环绕**：严防 2D 人像产生多眼多鼻或面部溶解；人像对峙镜头环绕严格限制在 **45° 以内（Subtle Arc）**。
3. **Z 轴纵深优先原则**：利用 *Slow Push-in*、*Crash Zoom*、*Dolly Zoom*、*Pull-out Reveal* 等沿进深方向运动，获得最高稳定性与视觉张力。
4. **2.5D 视差法则（强制前景遮挡）**：横移镜头必须强制植入近景/前景遮挡物（飞叶、雨丝、虚化肩膀、门框、火星），通过前快中慢后远的三层速度差制造立体 IMAX 级纵深。
5. **动能转移法则（人物微动态 + 摄影机重节奏）**：严格控制人物肢体大位移，将“爆发力与速度感”全权转移给**摄影机加速度（Speed Ramp）**、**剧烈焦点切换（Rack Focus）**与**快门动态模糊（Motion Blur）**。
6. **黑泽明三重运动法则（Kurosawa 3-Layer Motion）**：同时调动自然环境之动（风雨雷暴）、群体背景之动（军阵敌潮）与主体内心之动（眼眸杀气微颤）。

---

## 📽️ 运镜词库与光学技法矩阵 (Cinematography Matrix)

| 技法分类 | 核心术语 | 叙事功能与情绪暗示 |
| :--- | :--- | :--- |
| **推拉与变焦** | `Crash Zoom in` / `Whip Zoom` | 震惊、觉醒、杀气暴起、惊天秘密揭晓的瞬爆冲击 |
| **心理撕裂** | `Dolly Zoom` / `Vertigo Effect` | 希区柯克滑动变焦：背景扭曲形变而主体恒定，表现世界观崩溃、极度绝望 |
| **极度张力** | `The Leone Cut` | 赛尔乔·莱昂内剪辑：从极远广角全景瞬间跳切至眼眸大特写，引爆决战张力 |
| **同景深合成**| `Split Diopter Shot` | 双焦透镜：近处微距面孔与远处逼近的敌人同时保持极致锐利聚焦 |
| **空间穿梭** | `FPV Drone Dive & Corkscrew` | 穿越机垂直俯冲穿梭，展现宏大宗门、赛博都市与高速追逐 |
| **双人博弈** | `OTS Rack Focus` + `15° Arc` | 过肩微弧平移 + 焦点瞬间转移，表现猫捉老鼠般的权谋心理压制 |
| **身心沉浸** | `Snorricam / Chest Cam` | 身体固定机位：面部相对静止，背景疯狂震颤，表现逃亡与神魂颠乱 |
| **变速曲线** | `Speed Ramp Up` + `Impact Freeze` | 慢动作蓄势 $\rightarrow$ 瞬间加速冲撞 $\rightarrow$ 命中微定格打击感 |
| **电影光学** | `Anamorphic Oval Bokeh & Blue Flare` | 2.39:1 变形宽银幕横向蓝光条纹、椭圆焦外光斑与边缘微畸变 |

---

## 📐 五段式标准化输出格式 (Standard 5-Field Format)

每次执行分镜转换时，每个镜头（Shot）均严格对齐以下 5 个结构化字段：

```markdown
🎬 Shot [编号]：[镜头核心动作短标题]
1. 【景别与机位焦段】：明确景别（ECU/MCU/FS/WS） | 机位角度（Low-angle/Dutch Angle等） | 模拟焦段（如 24mm/85mm）
2. 【运镜轨迹与速度曲线】：起幅 -> 运动轨迹（Z轴/横移/弧形） -> 速度变化（Slow Dolly-in / Speed Ramp） -> 落幅
3. 【前/中/后景空间与光影】：前景遮挡视差 | 主体微动态 | 景深变化（Rack Focus / Shallow DOF） | 光影氛围
4. 【导演情绪动机】：一句话阐明运镜的戏剧叙事意图与心理暗示
5. 【AI 生视频英文 Prompt】：[Camera Angle & Shot Size], [Camera Movement & Speed], [Subject Micro-action & Foreground/Background], [Lighting, Depth of Field & Cinematic Style]
```

---

## 🤖 主流 AI 视频模型调优支持 (AI Video Model Matrix)

| 视频模型 | 最佳机位指令 | 动作幅度控制建议 | 避坑铁律 |
| :--- | :--- | :--- | :--- |
| **Minimax (海螺 / H3)** | `slow push-in`, `crash zoom`, `subtle camera shake`, `volumetric lighting` | 擅长景深氛围感、发丝衣摆微飘。人物避免复杂旋转。 | 避免输入复杂的多角色交替动作；优先指定单个主体的视线与微表情。 |
| **Seedance / Muse** | `parallax truck right`, `FPV dive`, `cinematic rim light`, `dynamic anime` | 动态漫画表现力极佳，擅长 2.5D 视差与光效流动。 | 严禁人物肢体大幅度拉伸，将冲击力交给光效粒子与背景移动。 |
| **Kling (快手可灵 1.5/2.0)** | `horizontal truck with foreground blur`, `low angle tilt up`, `dramatic speed ramp` | 动作连贯性强，擅长兵刃挥砍、气流与衣物摆动。 | 提示词开头必须严格前置机位角度与镜头类型，增强运镜依从性。 |
| **Runway Gen-3 Alpha** | `precise FPV tracking`, `dolly in`, `vertigo effect`, `masterpiece cinematic` | 影视级光影质感高，擅长逼真的镜头畸变与光晕。 | 提示词中明确写出 `rack focus from A to B`，模型能高度还原焦点变换。 |
| **即梦 (Jimeng / ByteDance)** | `slow dolly in`, `subtle handheld`, `dramatic anime chiaroscuro`, `4k octane render` | 画面细腻度高，对国漫/日漫风格的轮廓光与面部表情解析力极强。 | 避免过于抽象的修饰词，多使用具体的物理道具与环境光源描述。 |

---

## 🚀 安装与使用指南 (Installation & Usage)

### 1. Google Antigravity
克隆或复制本仓库到你的 Antigravity skills 目录：
```bash
# 全局生效安装：
mkdir -p ~/.gemini/config/skills/movie-camera-director
cp SKILL.md ~/.gemini/config/skills/movie-camera-director/

# 或在项目工程中生效：
mkdir -p .agents/skills/movie-camera-director
cp SKILL.md .agents/skills/movie-camera-director/
```

### 2. Claude Code / Codex / OpenClaw
```bash
# Claude Code 全局技能目录：
mkdir -p ~/.claude/skills/movie-camera-director
cp SKILL.md ~/.claude/skills/movie-camera-director/

# Codex 全局技能目录：
mkdir -p ~/.agents/skills/movie-camera-director
cp SKILL.md ~/.agents/skills/movie-camera-director/
```

---

## 📖 范例参考 (Examples)

查看 [`examples/`](examples/) 目录下的重构案例：
- [01 战斗爆发与杀气觉醒 (Combat Awakening)](examples/01_combat_awakening.md)
- [02 双人对峙与心智博弈 (Psychological Interrogation)](examples/02_psychological_interrogation.md)
- [03 惊悚绝境与世界颠覆 (Cosmic Horror Vertigo)](examples/03_cosmic_horror_vertigo.md)
- [04 双焦末日战场机甲逼近 (Split Diopter Mech Standoff)](examples/04_split_diopter_mech_standoff.md)

---

## 📄 License

MIT License © 2026 [Yiming Dong (dymx101)](https://github.com/dymx101).
