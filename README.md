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
🚀 How to Use
Write tasks in PromptDox format

Paste them into your GPT session

Let GPT process and auto-complete each task

🧠 Why PromptDox?
No special syntax to learn

Perfect for designers, developers, and AI beginners

Works well with GPT-4 / GPT-4-turbo

📂 Files
docs/spec-v1.1.md: Full Japanese specification

README.md: English project overview

👤 Author
PromptDox™
Created by [sakanakko]
Licensed under MIT

---

## ✅ ② docs/spec-v1.1.md（→ すでに用意済み！）

- さきほど作った「仕様書（日本語）」を `docs/spec-v1.1.md` に保存してアップすればOK！
- コマンド操作不要、GitHubの「Add file」から直接コピペでOKです。

---

## ✅ ③ GitHubリポジトリ名と構成（おすすめ）

- リポジトリ名: `promptdox`
- 構成：
/promptdox ├── README.md └── docs/ └── spec-v1.1.md

---

## 🔁 公開したらやってみたいこと（任意）

- ✅ 英語版 `spec-en.md` をあとで追加
- ✅ Shields.io バッジ追加（例：「version 1.1」「MIT License」）
- ✅ GitHub Topics に `#prompt-format` `#gpt` `#doxygen` を入れる
- ✅ README末尾に「使ってみた例」も載せられる

---

## 🚩最後に：公開用ライセンス（MIT）

```text
MIT License

Copyright (c) 2025 [あなた]

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction...

（以下省略。GitHubで「MIT License」選ぶだけで自動で入ります）

