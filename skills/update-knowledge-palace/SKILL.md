---
name: update-knowledge-palace
description: 专门用于创建、更新或维护本项目知识宫殿（Knowledge_Palace）的技能。在任何需求开发、产品设计或 Bug 修复完成后，或者用户明确要求“更新知识宫殿”、“同步文档”、“沉淀知识”、“执行 DoD”时，必须触发此技能，以确保代码与文档永远保持 100% 对齐！
---

# ✍️ 更新知识宫殿 (Update Knowledge Palace)

## 🎯 技能目标
在项目演进过程中，保持知识宫殿的内容与实际产品逻辑、代码架构 100% 实时同步。防止“死文档”的产生，落实 DoD (Definition of Done) 的最后一环。

## 🗺️ 更新原则与路径 (Progressive Disclosure)
你需要遵循“渐进式披露”的目录结构来更新文档，**不要破坏现有的网状索引结构**。

### 步骤 1：明确更新范围
1.  询问用户或自行判断本次迭代涉及了哪些改动：是新增了页面？修改了现有功能的交互？引入了新的状态管理？还是改变了后端 API？
2.  阅读 `Knowledge_Palace/04_QA_And_DoD/Definition_of_Done.md` 了解更新纪律。

### 步骤 2：执行渐进式更新
根据改动内容，定位并更新对应层级的文件。注意：**如果新增了独立模块或页面，必须创建新文件并在上一级的 Index/Inventory 目录中添加链接！**

*   **如果是【产品功能/交互的修改】**：
    1.  如果修改了已有页面：直接更新 `Knowledge_Palace/01_Product_Context/Features/` 下对应的 `.md` 文件。
    2.  如果新增了页面/大功能：在 `Features/` 下新建 `.md` 文件，并在 `Knowledge_Palace/01_Product_Context/Feature_Inventory.md` 中添加链接。
    3.  如果引入了新术语：更新 `Glossary.md`。

*   **如果是【代码映射/技术架构的修改】**：
    1.  如果修改了现有模块的依赖文件：更新 `Knowledge_Palace/03_Features_Detail/` 下对应模块的 `Traceability Matrix`（代码文件映射表）。
    2.  如果新增了业务模块：在 `03_Features_Detail/` 下新建 `.md` 文件，并在 `00_Module_Index.md` 中添加链接。
    3.  如果新增了 Zustand Store、修改了 API 契约或做出了重大架构决策：分别更新 `02_System_Architecture/` 下的 `State_Management.md`, `API_Contract.md`, 或在 `Decision_Records/` 下新增 ADR 文件。

### 步骤 3：验收汇报
*   更新完成后，向用户进行简短汇报，列出你具体修改了知识宫殿中的哪些文件。
*   汇报格式参考：
    > "✅ 知识宫殿已同步更新：
    > - 在 `Page_Reader.md` 中补充了 xxx 的交互规则。
    > - 在 `Module_Reader.md` 的代码映射表中添加了 `hooks/useReader.ts`。"
*   **注意**：必须使用**中文**进行汇报和文档撰写。
