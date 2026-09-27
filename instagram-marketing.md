# 📱 Ultimate Claude Instagram & Social Marketing Hub

> אוסף הסקילים, האוטומציות, הכלים וקישורי ה-GitHub המובילים לניהול אינסטגרם, הגדלת חשיפה, יצירת הוקים ויראליים ואוטומציות מכירה בעזרת **Claude AI**.

[![Instagram](https://img.shields.io/badge/Instagram-Viral_Marketing-E4405F?logo=instagram&logoColor=white)](https://instagram.com)
[![Claude](https://img.shields.io/badge/Claude-AI_Ecosystem-d97706?logo=anthropic)](https://claude.ai)
[![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

---

## 📑 תוכן עניינים
1. [🔗 קישורים וכלים מומלצים ב-GitHub](#-קישורים-וכלים-מומלצים-בגיטהב)
2. [🛠 סקילים מרכזיים לשיווק באינסטגרם](#-סקילים-מרכזיים-לשיווק-באינסטגרם)
3. [📊 טבלת כלי אוטומציה וניהול תוכן](#-טבלת-כלי-אוטומציה-וניהול-תוכן)
4. [🎥 פרומפטים מוכנים לקלוד ליצירת תוכן](#-פרומפטים-מוכנים-לקלוד-ליצירת-תוכן)

---

## 🔗 קישורים וכלים מומלצים ב-GitHub

הנה כמה מהריפוזיטוריים והכלים החזקים ביותר שקיימים כיום ברשת לשיווק ואוטומציה ברשתות חברתיות:
* **[ManyChat Automations & API Hub](https://github.com/topics/manychat)** — כלי ניהול ה-DM והתגובות האוטומטיות המוביל בעולם.
* **[Social Media Auto-Poster Python](https://github.com/topics/social-media-automation)** — סקריפטים בקוד פתוח לתזמון והעלאת פוסטים אוטומטית.
* **[OpenAI / Claude Copywriting Prompts](https://github.com/topics/prompt-engineering)** — מאגר פרומפטים מתקדמים לכתיבה שיווקית וקופי ויראלי.

---

## 🛠 סקילים מרכזיים לשיווק באינסטגרם

### 1. 🎣 Viral Hook Generator Skill
* **טכנולוגיה:** Prompt Engineering / Claude Project Instructions
* **ייעוד:** יצירת פתיחי וידאו עוצמתיים שגורמים לצופים להפסיק לגלול ב-3 השניות הראשונות.
* **מה הסקיל עושה:** מנתח את הנישה שלך ומייצר תבניות פתיחה פסיכולוגיות שמזניקות את אחוזי הצפייה (Retention Rate).

### 2. 🔄 Carousel Post Copywriting Agent
* **טכנולוגיה:** Structured Markdown / Design Prompts
* **ייעוד:** כתיבת תכנים לפוסט שקופיות (Carousel) שמובילים לשמירות ושיתופים רבים.
* **מה הסקיל עושה:** בונה שקף-אחר-שקף מבנה נרטיבי ברור: שקף פתיחה מסקרן, ערך פרקטי באמצע, והנעה לפעולה בסוף.

### 3. 🤖 DM Automation & Comment Bot Prompt
* **טכנולוגיה:** Make.com / ManyChat API Prompts
* **ייעוד:** ניהול שיחות אוטומטיות ב-Direct Messages לכל מי שמגיב למילה מסוימת בפוסט.
* **מה הסקיל עושה:** כותב תסריטי מענה חכמים שמובילים את הלקוח לרכישה או להשארת ליד באופן אוטומטי.

---

## 📊 טבלת כלי אוטומציה וניהול תוכן

| מטרה שיווקית | כלי / טכנולוגיה | סוג אינטגרציה | קישור חיצוני |
| :--- | :--- | :--- | :--- |
| **יצירת הוקים לרילס** | Claude AI Prompting | טקסט / פרומפט | [צפייה ↗](https://claude.ai) |
| **אוטומציית תגובות ו-DM** | ManyChat / Make.com | API / Webhook | [צפייה ↗](https://manychat.com) |
| **ניתוח האשטאגים ונישה** | Python Automation | סקריפט קוד | [GitHub ↗](https://github.com) |
| **תזמון פוסטים וסטוריז** | Meta Business Suite | רשמי | [צפייה ↗](https://business.facebook.com) |

---

## 💻 סקריפטים וכלים להעתקה

### קובץ סקיל לדוגמה: `instagram-growth-skill.md`
> העתק תוכן זה לקובץ חדש בריפו תחת תיקיית `instagram-marketing/skill.md`:

```python
# Instagram Hashtag & Niche Optimizer Agent Template
import random

def generate_viral_instagram_caption(hook, body, cta):
    """
    מייצר פוסט אינסטגרם מובנה הכולל הוק, גוף טקסט שיווקי והנעה לפעולה
    """
    hashtags = ["#AI", "#TechTrends", "#DigitalMarketing", "#BusinessGrowth", "#ClaudeAI", "#ContentCreator"]
    selected_tags = random.sample(hashtags, 4)
    
    caption = f"""
🔥 {hook}

-----------------------------------
{body}
-----------------------------------

👇 מה דעתך? ספר בתגובות!
{cta}

.
.
.
{' '.join(selected_tags)}
    """
    return caption.strip()

# דוגמה להפעלה:
# print(generate_viral_instagram_caption("כולם עושים את הטעות הזאת באינסטגרם!", "הנה 3 דרכים פשוטות לתקן את זה...", "תשמור את הפוסט כדי לא לאבד את זה!")
