---
name: query-knowledge-palace
description: 专门用于查询和调研本项目知识宫殿（Knowledge_Palace）的技能。当你需要进行新产品设计、了解现有功能、查阅技术架构或开始编写代码前，请使用此技能。当用户要求“调研知识宫殿”、“查一下现有功能”、“这个模块是怎么设计的”或类似问题时，请务必触发此技能！
---

# 📖 查询知识宫殿 (Query Knowledge Palace)

## 🎯 技能目标
在进行任何新需求设计或代码修改前，帮助 AI 快速、精准地获取项目的业务上下文、技术架构及代码文件映射关系。避免 AI 因为盲目阅读代码而产生幻觉或信息过载。

## 🗺️ 查阅路径 (Progressive Disclosure)
你需要遵循“渐进式披露”的原则来获取上下文，**严禁一开始就直接读取业务代码文件！**

### 步骤 1：定位入口
1. 始终从 `Knowledge_Palace/00_Index.md` 或 `Knowledge_Palace/AI_Bootstrap.md` 开始。
2. 根据用户的诉求，判断你需要的是【产品视角】还是【技术视角】。

### 步骤 2：判断诉求与下钻
*   **如果是【产品设计 / 需求调研】**：
    1. 查阅 `Knowledge_Palace/01_Product_Context/Feature_Inventory.md`，找到对应的功能目录。
    2. 下钻到 `Knowledge_Palace/01_Product_Context/Features/` 下的具体页面/功能文件，阅读交互细节与产品规则。
    3. 如果涉及整体业务闭环，阅读 `Core_Business.md`。

*   **如果是【代码开发 / 架构了解 / Bug 修复】**：
    1. 查阅 `Knowledge_Palace/03_Features_Detail/00_Module_Index.md`，找到对应的技术模块。
    2. 下钻到 `Knowledge_Palace/03_Features_Detail/` 下的具体模块文件（如 `Module_Reader.md`）。
    3. 找到该模块的 **代码文件级映射 (Traceability Matrix)**，**仅打开**表格中列出的相关源码文件（如 `.tsx`, `.ts`）。
    4. 如果需要了解全局技术约定或状态机结构，阅读 `02_System_Architecture/` 目录下的相关文件。

### 步骤 3：输出与答复
*   将你查询到的上下文整合后回答用户的问题。
*   在回答中，可以附带 Markdown 链接指向你查阅的知识宫殿文件，例如：*“根据 [Page_Reader.md](file:///Users/jiangjiahao/Documents/Workspace/PRD-Reader/Knowledge_Palace/01_Product_Context/Features/Page_Reader.md) 的定义，左侧树的触发机制是...”*
*   **注意**：所有回答必须使用**中文**。
