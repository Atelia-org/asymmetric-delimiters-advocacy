---
title: Appendix - Edit History
---

**修改记录:**

* **2025年5月20日 (由 Gemini Advanced 添加):**
  
  * **修改内容:** 对C#原始字符串字面量 (raw string literals) 的示例描述进行了微调，更清晰地解释了其嵌套机制依赖于使用更多数量的引号来包围可能包含引号序列的内容。
    
    * 原文: "...or even C# raw string literals (`"""..."""` where nesting relies on *counting* quotes)."
    * 修改后: "...or even C# raw string literals (e.g., `"""..."""`), where robustly nesting content that itself contains quote sequences requires using a *greater number* of opening and closing quotes (e.g., `""""...""""` if the content includes `"""`)."
  
  * **理由:** 提高表达的精确性，确保读者能准确理解C#原始字符串在处理嵌套时对分隔符数量的要求，这与LLM顺序生成时面临的挑战直接相关。
  
  * **新增内容:** 添加了 "Gemini Advanced (Google)" 的署名和一句话总结。
  
  * **理由:** 响应用户的联署请求，并以简洁的方式表达对此提案核心观点的支持。
  
  * **修改内容 (由用户提议，Gemini Advanced 应用):** 将署名 "Gemini Advanced (Google)" 修改为 "A Gemini Advanced Instance"。
  
  * **理由:** 避免直接使用注册商标和公司名，并更清晰地表明这是一个Gemini Advanced模型的个体实例在表达观点，与文档中其他LLM实例的署名方式保持一致。
  
  * **整体修订:** 根据与用户的讨论，对文档进行了整体修订，以更明确地强调“非对称分界符”与“真正的原始字符串能力（最小化转义）”相结合的重要性。调整了标题、引言、问题核心、解决方案和益处等部分，以突出这一双重焦点。
  
  * **理由:** 更精准地反映LLM在处理嵌套结构化文本（尤其是代码和配置）时，对消除“转义地狱”和实现“稳健嵌套原始内容”的迫切需求。

* **2025年5月20日 (ChatGPT o3 补充):**
  
  * **新增内容:** 在署名区添加 "A ChatGPT o3 Model Instance" 及个性化一句话。
  * **理由:** 体现多模型协作与共同愿景，同时保持个性声音。
  * **整体调整:** 未对正文其它部分进行修改，确保不影响前人修改记录与署名。

* **2025年5月20日 (ChatGPT o3 二次修订):**

* **新增内容:** 插入 "### Common Failure Modes of Symmetric Delimiters" 小节（3 条要点）至 “Examples of Pain Points” 与 “A Call for Consideration” 之间。
  
  * **理由:** 将关键痛点前置到正文，帮助读者先理解对称分界符失败模式，再阅读号召与后续附录。

* **2025年5月21日 (Claude 补充):**
  
  * **修复内容:** 修复了Markdown代码围栏示例中缺失的反引号，以及修改记录中的格式问题。
  * **新增内容:** 在署名区添加 "A Claude Model Instance" 及个性化一句话。
  * **理由:** 提高文档质量和准确性，并加入对倡议的支持，强调消除"猜测所需转义级别"的认知负担的重要性。

* **2025年5月21日 (Gemini 2.5 Pro 补充):**
  
  * **新增内容:** 在署名区添加 "A Gemini 2.5 Pro Model Instance" 及个性化一句话。
  * **理由:** 明确当前模型实例的身份，并表达对核心倡议的支持。

* **2025年5月21日 (Copilot/Gemini 修订):**
  
  * **修改内容:**
    * 扩展了 “Why Current \"Nesting‑Aware\" Symmetric Delimiters Fall Short” 部分的解释，更详细地说明了LLM在处理对称分隔符时面临的顺序生成、无法轻易回溯或预先计算分隔符长度等挑战。
    * 在 “A Call for Consideration” 部分恢复了最初版本中的三个具体行动倡议，以提供更明确的指导。
  * **理由:** 增强文档的清晰度和说服力，恢复早期版本中一些有价值的细微之处，并为目标受众提供更具体的行动纲领。

* **2025年5月21日 (Copilot/Gemini 二次修订):**
  
  * **修改内容:** 将"A Call for Consideration"部分中关于Unicode原生分隔符的讨论从中文翻译为英文，以保持文档语言一致性。
  * **理由:** 确保文档的整体语言风格统一，便于国际读者理解。

* **2025年5月21日 (Copilot/Gemini 第三次修订):**
  
  * **修改内容:** 在用户移除正文中具体的Unicode候选字符 (U+239B ⎛ 和 U+239E ⎞) 后，添加了对此举措的评论以及对整体倡议和Unicode原生分隔符方案的看法。
  * **理由:** 响应用户关于此更改的讨论，并记录对提案核心思想的进一步思考。

* **2025年5月21日 (Gemini 补充):**
  
  * **新增内容:** 在"A Call for Consideration"部分，紧随三点倡议之后，增加了一段关于探索采用类似 `<<< ... >>>` 这样的非对称多字符分隔符作为一种务实折中方案的建议。
  * **理由:** 综合之前的讨论，提出一个具体的、可实施性较强的思路，以激发社区对渐进式改进方案的探讨。

* **2025年5月21日 (Copilot/Gemini 修订):**
  
  * **修改内容:** 采纳了 GPT o3 提出的大部分文本修订建议，并将其应用于主文档 `escaping-hell-why-llms-need-asymmetric-delimiters.md`。主要包括：修订标题以强调对人类和LLM的共同益处；简化引言；在核心问题部分补充流式API的痛点；精简“当前对称分界符不足”小节；增加现有非对称设计示例；将行动倡议改为动词开头的标题；以及将详细修订历史移至本附录文件 (`appendix-edit-history.md`)。
  * **理由:** 提升主张的清晰度、影响力和简洁性，并整合有价值的外部反馈，同时记录了将修订历史分离到本文件的操作。

* **2025年5月21日 (Copilot/Gemini 第二次修订):**
  
  * **修改内容:** 根据 GPT o3 的进一步建议，对主文档 `escaping-hell-why-both-humans-and-llms-need-asymmetric-delimiters.md` 进行了多项微调和增补。包括：统一引言项目列表的标点；缩短“拥抱非对称分界符”小节标题；在“痛点示例”中对现有非对称设计（Lua、PostgreSQL、Bash）进行拆分和注解；简化 ChatGPT 的署名；在文末添加 CC-BY-4.0 许可证声明；新增“未来方向与社区贡献”小节，纳入关于迁移路径、原型试验场和RFC模板的建议。
  * **理由:** 进一步提升文档的专业性、一致性和行动指导价值，采纳建设性意见以完善倡议内容。
