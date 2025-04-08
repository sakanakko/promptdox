# PromptDox™

A Doxygen-inspired structured prompt format for GPT agents.  
Write what you want the AI to do—clearly, repeatably, and automatically.

📘 [Spec v1.1 - 日本語仕様書はこちら](docs/spec-v1.1.md)

---

## ✨ What is PromptDox?

**PromptDox™** is a lightweight, GPT-friendly format for describing AI tasks using annotated comments.  
It lets you write instructions like source code documentation—and the AI understands and executes them.

> ✅ Easy to write  
> ✅ Supports multiple tasks  
> ✅ Human-readable, machine-actionable  

---

## 📐 Example PromptDox (Multi-task)

```cpp
/**
 * @promptdox_list
 * @version 1.1
 * @auto_execute true
 */

/**
 * @task spring_background
 * @brief Create a spring fashion background
 * @details
 * - Size: 640x640
 * - Pastel watercolor with lace
 * - Seamless PNG, transparent
 * @output image
 */

/**
 * @task logo_frame
 * @brief Frame image for photos
 * @details
 * - Size: 800x1600
 * - Spring-like decor, center blank
 * @output image
 */
# promptdox
Doxygen-inspired task prompt format for AI systems
