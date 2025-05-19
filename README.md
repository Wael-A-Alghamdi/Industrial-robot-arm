# Industrial Robot Arm Project

This is a simple IoT project to control a 6-motor industrial robot arm using a web-based interface. The system includes:

- A front-end control panel built in HTML and CSS 
- A PHP script to handle database communication  
- A MySQL database to store motor positions and robot status 

The project was originally built for practice and demonstration purposes.

---

## 🔗 Live Demo  
[Open the Control Panel](https://wael-a-alghamdi.github.io/Industrial-robot-arm/industrial_robot_arm_project_1.html)

---

## 🔧 Tech Used  
- HTML  
- CSS  
- PHP  
- MySQL  

---

## ⚠️ Notes  
- Fully static front-end — no JS frameworks.  
- PHP handles form submissions and writes to the database.  
- The robot has 6 motors, each controlled via a slider (0 to 180 degrees).  
- The database contains two tables: `engines` and `run`.  
- You need a local server (e.g. XAMPP) to run `connect.php` and access the MySQL database.  
- Includes a background image (`html_background_image.jpg`) used in the HTML page.

---

## 📁 Project Files  
- `industrial_robot_arm_project_1.html` – Control interface  
- `connect.php` – PHP backend for form processing  
- `industrial_robot_arm__project_1_database.sql` – SQL dump of the database  
- `html_background_image.jpg` – Background image used in the HTML  
- `README.md` – Project documentation  

---

## 🧾 Project Overview (Arabic + English)

### 📌 المقدمة – Introduction

في هذا المشروع قمت بإنشاء صفحة تحكم (HTML) لذراع روبوت صناعي مكون من 6 محركات، وقاعدة بيانات لتخزين القيم، وربطت بينهم باستخدام صفحة (PHP).  
In this project, I created an HTML page to control a robot arm, created a database, and linked them using a PHP page.

---

### 1. إنشاء صفحة HTML – Create HTML Page

- الصفحة تتكون من 6 منزلقات (Sliders) للتحكم في كل محرك من 0 إلى 180 درجة  
- تحتوي على 3 أزرار: حفظ – تشغيل – إيقاف  
- تم استخدام CSS لتنسيق الصفحة وجعلها أكثر وضوحًا  
The HTML page includes six motor controls, a save button, a run button, and a stop button. Styling was done using plain CSS.

---

### 2. إنشاء قاعدة البيانات – Create the Database

تم إنشاء قاعدة بيانات مكونة من جدولين:

- جدول `engines`: يحتوي على 6 أعمدة للمحركات وعمود `id` كمفتاح أساسي  
- جدول `run`: يحتوي على أعمدة لحالة التشغيل/الإيقاف وعمود `id` كمفتاح أساسي  
The database has two tables:  
- `engines`: Stores motor angles (engineOne to engineSix)  
- `run`: Stores on/off status of the robot  

---

### 3. الربط بين HTML وقاعدة البيانات – Connecting HTML to the Database

- تم استخدام `connect.php` لكتابة كود الاتصال وقبول البيانات من الصفحة  
- عند الضغط على زر حفظ أو تشغيل أو إيقاف، يتم إرسال القيم إلى قاعدة البيانات مباشرة  
Using the PHP file, form values are submitted and stored in the MySQL database depending on which button is pressed.

---
