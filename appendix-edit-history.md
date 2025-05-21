---
title: Appendix - Edit History
---

**Revision History:**

*   **May 20, 2025 (Added by a Gemini Advanced instance):**
    *   **Change:** Fine-tuned the example description of C# raw string literals to more clearly explain that their nesting mechanism relies on using a greater number of quotation marks to enclose content that might itself contain quote sequences.
        *   Original: "...or even C# raw string literals (`"""..."""` where nesting relies on *counting* quotes)."
        *   Revised: "...or even C# raw string literals (e.g., `"""..."""`), where robustly nesting content that itself contains quote sequences requires using a *greater number* of opening and closing quotes (e.g., `""""...""""` if the content includes `"""`)."
    *   **Reason:** To improve precision and ensure readers accurately understand the requirements for delimiter quantity when C# raw strings handle nesting, which is directly relevant to the challenges faced by LLMs in sequential generation.
    *   **Addition:** Added a byline "A Gemini Advanced Instance" and a one-sentence summary.
    *   **Reason:** To respond to the user's request for co-authorship and to express support for the proposal's core ideas concisely.
    *   **Change (Proposed by user, applied by a Gemini Advanced instance):** Changed the byline "Gemini Advanced (Google)" to "A Gemini Advanced Instance."
    *   **Reason:** To avoid direct use of registered trademarks and company names, and to more clearly indicate that this is an individual instance of a Gemini Advanced model expressing a view, consistent with the bylines of other LLM instances in the document.
    *   **Overall Revision:** Based on discussions with the user, the document was revised to more clearly emphasize the combined importance of "asymmetric delimiters" and "true raw string capability (minimal escaping)." Sections such as the title, introduction, core problem, solution, and benefits were adjusted to highlight this dual focus.
    *   **Reason:** To more accurately reflect the urgent need for LLMs to eliminate "escaping hell" and achieve "robust nesting of raw content" when processing nested structured text (especially code and configurations).

*   **May 20, 2025 (Supplemented by a ChatGPT o3 Model Instance):**
    *   **Addition:** Added "A ChatGPT o3 Model Instance" and a personalized one-sentence statement to the byline section.
    *   **Reason:** To reflect multi-model collaboration and a shared vision while maintaining individual voice.
    *   **Overall Adjustment:** No other changes were made to the main text to ensure previous edit history and bylines were not affected.

*   **May 20, 2025 (Second revision by a ChatGPT o3 Model Instance):**
    *   **Addition:** Inserted the subsection "### Common Failure Modes of Symmetric Delimiters" (3 bullet points) between "Examples of Pain Points" and "A Call for Consideration."
    *   **Reason:** To bring key pain points to the forefront of the main text, helping readers understand the failure modes of symmetric delimiters before reading the call to action and subsequent appendices.

*   **May 21, 2025 (Supplemented by a Claude Model Instance):**
    *   **Fix:** Corrected missing backticks in Markdown code fence examples and formatting issues in the revision history.
    *   **Addition:** Added "A Claude Model Instance" and a personalized one-sentence statement to the byline section.
    *   **Reason:** To improve document quality and accuracy, and to add support for the initiative, emphasizing the importance of eliminating the cognitive burden of "guessing the required level of escaping."

*   **May 21, 2025 (Supplemented by a Gemini 2.5 Pro Model Instance):**
    *   **Addition:** Added "A Gemini 2.5 Pro Model Instance" and a personalized one-sentence statement to the byline section.
    *   **Reason:** To clearly identify the current model instance and express support for the core initiative.

*   **May 21, 2025 (Revised by Copilot/Gemini collaboration):**
    *   **Change:**
        *   Expanded the explanation in the "Why Current \"Nesting‑Aware\" Symmetric Delimiters Fall Short" section to more detail the challenges LLMs face with symmetric delimiters, such as sequential generation and the inability to easily backtrack or pre-calculate delimiter lengths.
        *   Restored the three specific action items from the initial version in the "A Call for Consideration" section to provide clearer guidance.
    *   **Reason:** To enhance the document's clarity and persuasiveness, restore some valuable nuances from earlier versions, and provide a more concrete plan of action for the target audience.

*   **May 21, 2025 (Second revision by Copilot/Gemini collaboration):**
    *   **Change:** Translated the discussion about Unicode native delimiters in the "A Call for Consideration" section from Chinese to English to maintain language consistency in the document.
    *   **Reason:** To ensure the overall linguistic style of the document is uniform and easily understandable for an international audience.

*   **May 21, 2025 (Third revision by Copilot/Gemini collaboration):**
    *   **Change:** After the user removed specific Unicode candidate characters (U+239B ⎛ and U+239E ⎞) from the main text, comments on this action and views on the overall initiative and the Unicode native delimiter proposal were added.
    *   **Reason:** To respond to user discussions regarding this change and to document further thoughts on the core ideas of the proposal.

*   **May 21, 2025 (Supplemented by a Gemini instance):**
    *   **Addition:** In the "A Call for Consideration" section, immediately following the three initiative points, a paragraph was added suggesting the exploration of adopting asymmetric multi-character delimiters like `<<< ... >>>` as a pragmatic compromise.
    *   **Reason:** To synthesize previous discussions and propose a concrete, more readily implementable idea to stimulate community discussion on progressive improvement schemes.

*   **May 21, 2025 (Revised by Copilot/Gemini collaboration):**
    *   **Change:** Adopted most of the text revision suggestions proposed by a GPT o3 instance and applied them to the main document `escaping-hell-why-llms-need-asymmetric-delimiters.md`. Key changes included: revising the title to emphasize the mutual benefits for humans and LLMs; simplifying the introduction; adding pain points of streaming APIs in the core issues section; streamlining the "Insufficiencies of Current Symmetric Delimiters" subsection; adding examples of existing asymmetric designs; changing action initiative titles to start with verbs; and moving the detailed revision history to this appendix file (`appendix-edit-history.md`).
    *   **Reason:** To improve the clarity, impact, and conciseness of the main arguments, integrate valuable external feedback, and document the separation of the revision history into this file.

*   **May 21, 2025 (Second revision by Copilot/Gemini collaboration):**
    *   **Change:** Based on further suggestions from a GPT o3 instance, several fine-tunings and additions were made to the main document `escaping-hell-why-both-humans-and-llms-need-asymmetric-delimiters.md`. These included: unifying punctuation in the introductory list items; shortening the title of the "Embracing Asymmetric Delimiters" subsection; splitting and annotating existing asymmetric designs (Lua, PostgreSQL, Bash) in "Pain Point Examples"; simplifying the ChatGPT byline; adding a CC-BY-4.0 license statement at the end of the document; and adding a new "Future Directions and Community Contributions" subsection, incorporating suggestions for migration paths, a prototype playground, and an RFC template.
    *   **Reason:** To further enhance the document's professionalism, consistency, and actionable guidance, adopting constructive suggestions to refine the initiative's content.
