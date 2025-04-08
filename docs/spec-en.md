# PromptDox-List: Structured Prompt Format Specification (v1.1)

## 📘 Overview
**PromptDox-List** is a lightweight, GPT-friendly format inspired by Doxygen. It allows users to describe multiple tasks in a structured, readable format that GPT can understand and execute.

---

## ✅ Purpose

- Structure multiple instructions in a single prompt
- Clearly define each task's goal, detail, and output type
- Auto-execute tasks if `@auto_execute` is enabled

---

## 📐 Basic Syntax

```cpp
/**
 * @promptdox_list
 * @version 1.1
 * @auto_execute true
 */

/**
 * @task task_id_or_name
 * @brief One-line task summary
 * @details
 * - Key requirements
 * - Style, format, etc.
 * @output image / text / code
 */
```

---

## 🧠 GPT Interpretation Flow

1. Detects `@promptdox_list` → enters multi-task mode
2. Parses each `@task` block one by one
3. Executes task based on `@output` type
4. Automatically processes tasks if `@auto_execute` is set to true
5. Can internally mark tasks as completed (future enhancement)

---

## 🧩 Available Tags

| Tag             | Description                                     |
|----------------|-------------------------------------------------|
| `@promptdox_list` | Marks the start of a multi-task list           |
| `@version`        | Format version                                 |
| `@auto_execute`   | true/false to allow automatic task execution   |
| `@task`           | Unique ID or name for each task                |
| `@brief`          | Short summary of the task                      |
| `@details`        | Detailed task description (list or text)       |
| `@output`         | Output type (image, text, code, etc.)          |

---

## 📝 Example Prompt

```cpp
/**
 * @promptdox_list
 * @version 1.1
 * @auto_execute true
 */

/**
 * @task spring_background
 * @brief Spring fashion POP background
 * @details
 * - Size: 640x640
 * - Pastel watercolor, soft lace pattern
 * - PNG format, transparent, seamless
 * @output image
 */

/**
 * @task logo_frame
 * @brief Logo frame for photo
 * @details
 * - Size: 800x1600
 * - Decorative edges, center left blank
 * @output image
 */

/**
 * @task headline_text
 * @brief Headline text image
 * @details
 * - Text: Spring Lace Item Feature
 * - Size: 1536x97
 * - Font: gentle and feminine
 * - Format: PNG with transparency
 * @output image
 */
```

---

## 🔮 Future Tag Extensions

| Tag             | Purpose                                          |
|----------------|--------------------------------------------------|
| `@priority`     | Execution priority (high / medium / low)         |
| `@depends_on`   | Task dependencies                                |
| `@group`        | Category tag (image / text / system)             |
| `@deadline`     | Optional execution deadline (e.g., 2025-04-10)   |

---

## 👤 Author

```
PromptDox™ - Structured Prompt Format for GPT Tasks  
Created by: Community Developers  
Version: 1.1 / April 2025
```

---

## 🌍 Use Cases

- Notion or GitHub integrated AI workflows  
- GPT-4-turbo prompt engineering  
- Task list automation and documentation

---

## 🔁 Beginner-Friendly Template

```
Please write the following tasks in PromptDox-List format.  
Set `@auto_execute true` and output as images.

[Task List]
1. Spring-themed seamless background (640x640)
2. Transparent photo frame (800x1600)
3. Headline image: "Spring Lace Item Feature" (1536x97)
```

