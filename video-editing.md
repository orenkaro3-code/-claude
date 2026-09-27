# 🎬 Claude Video Editing & Multimedia Hub

> אוסף הסקילים, האוטומציות והכלים המתקדמים ביותר לשליטה בעריכת סרטונים, יצירת אנימציות קוד וניצול כלי AI וידאו בעזרת **Claude AI**.

[![Claude](https://img.shields.io/badge/Claude-Video_Agent-d97706?logo=anthropic)](https://claude.ai)
[![Remotion](https://img.shields.io/badge/Remotion-Code_Video-blue?logo=react)](https://www.remotion.dev/

---

## 📑 תוכן עניינים
1. [סקילים מרכזיים לעריכת וידאו](#-סקילים-מרכזיים-לעריכת-וידאו)
2. [סקריפטים וכלים להורדה והעתקה](#-סקריפטים-וכלים-להעתקה)
3. [פרומפטים להפקת סרטונים ב-AI](#-פרומפטים-לבימוי-והפקת-וידאו)

---

## 🛠 סקילים מרכזיים לעריכת וידאו

### 1. 🎞️ Remotion Code-Video Skill
* **טכנולוגיה:** React + Remotion
* **ייעוד:** יצירת סרטוני תוכנה, אנימציות קוד וסרטונים מורכבים באופן פרוגרמטי דרך קלוד.
* **מה הסקיל עושה:** מאפשר לקלוד לכתוב קומפוננטות React שמתרנדרות לסרטון MP4 חלק ברזולוציה גבוהה.

### 2. ✂️ FFmpeg Video Automation Agent
* **טכנולוגיה:** Python + FFmpeg CLI
* **ייעוד:** חיתוך, מיזוג, הוספת כתוביות והמרת פורמטים לסרטונים באופן אוטומטי לחלוטין.
* **מה הסקיל עושה:** קלוד כתוכנת עריכה בטרמינל – מזהה קטעי וידאו, גוזר את החלקים הטובים ומחבר מוזיקת רקע.

### 3. 📱 Reels & TikTok Auto-Subtitles Skill
* **טכנולוגיה:** Python + Whisper AI + Video Py
* **ייעוד:** הוספת כתוביות דינמיות בולטות (כמו בסרטונים ויראליים) אוטומטית.
* **מה הסקיל עושה:** מנתח את האודיו של הסרטון, מייצר קובץ כתוביות `SRT` אוטומטי וצורב אותן בעיצוב מודרני.

---

## 💻 קוד וסקריפטים לעריכה אוטומטית

```python
import subprocess

def crop_video_to_vertical(input_path, output_path):
    """
    חותך אוטומטית סרטון לפורמט אנכי (9:16) מתאים לאינסטגרם רילס ושורטס
    """
    cmd = [
        "ffmpeg", "-i", input_path,
        "-vf", "crop=ih*9/16:ih",
        "-c:a", "copy",
        output_path,
        "-y"
    ]
    result = subprocess.run(cmd, capture_output=True, text=True)
    if result.returncode == 0:
        print(f"Success! Vertical video saved to: {output_path}")
    else:
        print(f"Error: {result.stderr}")
