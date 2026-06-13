# 🤖 Project 1: Rule-Based AI Chatbot
**DecodeLabs Industrial Training Kit | Batch 2026**

---

## 📌 What This Project Is
A rule-based chatbot built in pure Python — no libraries, no ML, just control flow and logic. This is the **foundation of all AI systems**: before a machine can learn, someone must teach it rules explicitly.

---

## 🧠 Core Concepts Used

| Concept | What It Does |
|---|---|
| `while True` loop | Keeps the bot alive (the heartbeat) |
| Input sanitization | `.lower().strip()` makes input case-insensitive |
| Dictionary (Hash Map) | Stores all rules as `{ "input": "response" }` |
| `.get(key, fallback)` | O(1) lookup + handles unknown inputs gracefully |
| `break` | The kill command — exits the infinite loop |
| `if __name__ == "__main__"` | Standard Python entry point |

---

## ⚡ Why Dictionary over If-Elif?

| Approach | Complexity | Scalability |
|---|---|---|
| If-Elif Ladder | O(n) — checks every rule | Breaks down at scale |
| Dictionary `.get()` | O(1) — instant lookup | Scales to 10,000+ rules |

---

## 🏗️ Architecture: The IPO Model

```
INPUT          →        PROCESS         →       OUTPUT
(Raw Feed)           (Logic Skeleton)        (Feedback Loop)

raw_input            intent matching          print reply
.lower().strip()     dict.get(key)            loop continues
```

---

## 🚀 How to Run

```bash
python3 chatbot.py
```

**Sample commands to try:**
- `hello` / `hi` / `hey`
- `who are you`
- `what is ai`
- `tell me a joke`
- `help`
- `exit` / `quit` / `bye`

---

## 📁 Project Structure

```
project-1-chatbot/
└── chatbot.py      # Main chatbot script
└── README.md       # This file
```

---

## 🔮 What's Next (Project 2)
Moving from **exact key matching** (discrete/rigid) to **semantic/vector matching** — where the bot understands *meaning*, not just exact words.

---

*Built at DecodeLabs | Powered by pure Python logic 🐍*
