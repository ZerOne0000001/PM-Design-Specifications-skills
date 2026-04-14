# 设计倾向指南 (Design Trend Guide)

**这是写给后续前端生成节点（如 `frontend-design` 技能）的作战指令。**
**核心目的**：杜绝“AI塑料感”、“通用后台灰”等平庸设计，提供极端化、个性化且极具辨识度的视觉抓手。

## 1. 设计核心策略 (Design Core Strategy)

*   **设计理念 (Concept)**：[此处填写一句话总结，例如：复古未来主义与现代极简的碰撞]
*   **整体调性 (Tone)**：[必须使用极端词汇描述，例如：冷峻的、高对比度的、杂志般排版的、粗野主义的]
*   **差异化视觉锚点 (Visual Hook)**：[指出让用户过目不忘的 1-2 个特征，例如：超大号的标题排版，或者不对称的网格切割]

## 2. 字体与排版 (Typography)

*   **主标题 (Headings)**：
    *   **字体族 (Font Family)**：[例如：Playfair Display / 衬线体 / 超大字重无衬线体]
    *   **排版特征 (Characteristics)**：[例如：极紧凑的字间距（tracking-tighter），全大写，或是超大字号（text-7xl/8xl）]
*   **正文 (Body Text)**：
    *   **字体族 (Font Family)**：[例如：Inter / Roboto / 易读性极高的无衬线体]
    *   **排版特征 (Characteristics)**：[例如：宽松的行高（leading-relaxed），柔和的灰度（text-gray-600）]

## 3. 色彩与主题 (Color & Theme)

*   **主色调 (Primary Color)**：[给出具体的 Tailwind 类名或 Hex 值，例如：#E63946（警示红）或 bg-zinc-900（极深邃的黑）]
*   **辅助色 (Accent Color)**：[例如：高饱和度的荧光绿（text-lime-400），用于点缀]
*   **背景与暗黑模式 (Background & Dark Mode)**：[明确背景处理方式，例如：拒绝纯白，使用带有微弱暖调的 bg-stone-50；或者要求强制全局暗黑模式]
*   **边框与阴影 (Borders & Shadows)**：[例如：拒绝柔和阴影，强制使用 2px 的硬质纯黑边框（border-2 border-black）和无模糊的硬阴影（box-shadow: 4px 4px 0px #000）]

## 4. 空间组合与微交互 (Spatial Composition & Micro-interactions)

*   **网格与留白 (Grid & Spacing)**：[例如：打破常规对称，使用极度夸张的留白（p-24），或者极度紧凑的无缝拼接]
*   **圆角处理 (Border Radius)**：[例如：绝对直角（rounded-none），或者极度圆滑的药丸状（rounded-full）]
*   **核心交互动效 (Key Interactions)**：[例如：按钮 Hover 时必须有明显的位移（translate-x-1 translate-y-1）或者背景色的瞬间反转]

---
**给 AI 生成器的强制提示**：
你（生成代码的大模型）在输出 Tailwind 类名或编写 CSS 时，**必须严格映射**上述要求。如果你敢使用默认的 `bg-blue-500` 或 `rounded-md` `shadow-md` 等平庸组件组合，将被视为严重失败！