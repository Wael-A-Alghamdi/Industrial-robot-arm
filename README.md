# Industrial Robot Arm Project

This is a basic front-end + backend project to control a robot arm via the web. Built using HTML, PHP, and MySQL. The project includes a database with engine values and robot run state.

---

🔧 Tech Used  
HTML  
CSS  
PHP  
MySQL  

---

⚠️ Notes  
- The control panel supports 6 motors using sliders (0–180 degrees).  
- PHP handles data submission and writes to the database.  
- `connect.php` connects the interface to the database.  
- Database has 2 tables: `engines` (for motor positions) and `run` (for robot on/off status).  
- Background image is loaded locally (make sure `html_background_image.jpg` is in the correct folder).  
- To run this project locally, you’ll need XAMPP or similar (Apache + MySQL).

---

Files Overview  
- `industrial_robot_arm_project_1.html` – Web control panel  
- `connect.php` – Server-side logic to save input to DB  
- `industrial_robot_arm__project_1_database.sql` – SQL dump to create tables and sample data  
- `html_background_image.jpg` – Background for the control page  
