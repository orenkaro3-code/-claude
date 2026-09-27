# 🌐 Ultimate Claude Web Development & UI/UX Hub

> אוסף הסקילים, האוטומציות, הכלים וקישורי ה-GitHub המובילים לבניית אתרים מתקדמים, אנימציות WebGL / Three.js, ומערכות עיצוב (UI/UX) בעזרת **Claude AI**.

[![Web Dev](https://img.shields.io/badge/Web_Dev-Fullstack_%2F_3D-blue?logo=react&logoColor=white)](https://github.com/topics/web-development)
[![Claude](https://img.shields.io/badge/Claude-AI_Agent-d97706?logo=anthropic)](https://claude.ai)
[![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

---

## 📑 תוכן עניינים
1. [🔗 קישורים וריפוזיטוריים מובילים ב-GitHub](#-קישורים-וריפוזיטוריים-מובילים-בגיטהב)
2. [🛠 סקילים מרכזיים לבניית אתרים מתקדמים](#-סקילים-מרכזיים-לבניית-אתרים-מתקדמים)
3. [📊 טבלת ספריות וטכנולוגיות מומלצות](#-טבלת-ספריות-וטכנולוגיות-מומלצות)
4. [💻 קוד וסקריפטים להעתקה (Three.js / HTML)](#-קוד-וסקריפטים-להעתקה-threejs--html)
5. [🎥 פרומפטים מוכנים לקלוד לבניית אתרים](#-פרומפטים-מוכנים-לקלוד-לבניית-אתרים)

---

## 🔗 קישורים וריפוזיטוריים מובילים ב-GitHub

הנה כמה מהפרויקטים והסקילים החזקיים ביותר ברשת לפיתוח אתרים ואנימציות עם קלוד:
* **[WebGPU Claude Skill](https://github.com/dgreenheck/webgpu-claude-skill)** — פיתוח אפליקציות WebGPU ו-Three.js מתקדמות.
* **[Motion Web Creative](https://github.com/feitangyuan/motion-web)** — אתרי תדמית עם פיזיקה חיה ואנימציות גלילה מרשימות.
* **[Genjutsu Creative Coding](https://github.com/AThevon/genjutsu)** — סקילים של קלוד למיקרו-אינטראקציות, GSAP ומערכות עיצוב.
* **[Three.js Skill Package](https://github.com/Impertio-Studio/Three.js-Claude-Skill-Package)** — מארז של 24 סקילים מקצועיים לפיתוח 3D בדפדפן.

---

## 🛠 סקילים מרכזיים לבניית אתרים מתקדמים

### 1. 🌟 Award-Winning 3D Website Agent
* **טכנולוגיה:** Three.js / React Three Fiber / GSAP
* **ייעוד:** יצירת אתרי נחיתה אינטראקטיביים ברמת Awwwards עם תנועה ואנימציות חלקות.
* **מה הסקיל עושה:** מנחה את קלוד לבנות קומפוננטות ריאקטיביות, לשלב תאורה מתקדמת (Lighting) וניהול מעברי עמודים מדהימים.

### 2. ⚡ WebGL Shaders & GPU Optimization Skill
* **טכנולוגיה:** GLSL Shaders / WebGL
* **ייעוד:** כתיבת אפקטים חזותיים מיוחדים על כרטיס המסך (GPU) ישירות מהדפדפן.
* **מה הסקיל עושה:** מייצר קוד הצללה (Shaders) שנותן מראה סייברפאנקי, נוזלי או עתידני לאתר.

### 3. 📱 Fullstack React & Tailwind Architecture
* **טכנולוגיה:** Next.js / Tailwind CSS / Shadcn UI
* **ייעוד:** בניית אתרים רספונסיביים מלאים, מהירים ונגישים מקצה לקצה.
* **מה הסקיל עושה:** מוודא שקלוד כותב קוד נקי, מודולרי, המותאם ל-SEO ולביצועים מקסימליים (Lighthouse 100).

---

## 📊 טבלת ספריות וטכנולוגיות מומלצות

| מטרה פיתוחית | טכנולוגיה מרכזית | רמת מורכבות | קישור ב-GitHub |
| :--- | :--- | :--- | :--- |
| **אנימציות גלילה** | GSAP / Motion | בינוני | [צפייה ↗](https://github.com/topics/gsap) |
| **תלת-ממד בדפדפן** | Three.js / R3F | מתקדם | [צפייה ↗](https://github.com/topics/threejs) |
| **עיצוב וסטיילינג** | Tailwind CSS v4 | קל - בינוני | [צפייה ↗](https://github.com/topics/tailwindcss) |
| **גרפיקת קצה** | WebGPU / WGSL | מומחה | [צפייה ↗](https://github.com/topics/webgpu) |

---

## 💻 קוד וסקריפטים להעתקה

### קובץ סקיל לדוגמה: `threejs-hero-scene.js`
> תבנית Three.js בסיסית שקלוד משתמש בה כדי להוסיף קובייה תלת-ממדית מסתובבת לאתר שלך:

```javascript
import * as THREE from 'three';

// יצירת סצנה, מצלמה ורנדרר
const scene = new THREE.Scene();
const camera = new THREE.PerspectiveCamera(75, window.innerWidth / window.innerHeight, 0.1, 1000);
const renderer = new THREE.WebGLRenderer({ antialias: true, alpha: true });

renderer.setSize(window.innerWidth, window.innerHeight);
document.body.appendChild(renderer.domElement);

// יצירת אובייקט תלת-ממדי (קוביה)
const geometry = new THREE.BoxGeometry(2, 2, 2);
const material = new THREE.MeshStandardMaterial({ color: 0xd97706, roughness: 0.2 });
const cube = new THREE.Mesh(geometry, material);
scene.add(cube);

// הוספת תאורה
const light = new THREE.DirectionalLight(0xffffff, 2);
light.position.set(5, 5, 5);
scene.add(light);

camera.position.z = 5;

// לוגיקת אנימציה
function animate() {
    requestAnimationFrame(animate);
    cube.rotation.x += 0.01;
    cube.rotation.y += 0.01;
    renderer.render(scene, camera);
}
animate();
