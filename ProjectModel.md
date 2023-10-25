## 🚀 **ATLASs Project Model** 🚀

### 🎯 **Objective:**
To create an Automated Time, Location, and Attendance Analysis System for monitoring and managing student attendance efficiently using QR code scanning and real-time notifications.

### 🌐 **Components:**
1. **Admin Website**
2. **Mobile App**
3. **IoT Interface**
4. **Web Server**

### 📜 **Features and Functions:**

#### 🛠️ **Admin Account**
- Add new student.
- Assign timetable individually and in batch.
- Assign batches and sections to students.
- View individual student's attendance.
- View attendance for a particular course.
- Generate attendance report in PDF.

#### 👩‍🏫 **Teacher Account**
- View students assigned to them.
- Monitor attendance of each student.
- Edit class timings.
- Generate attendance reports.

#### 🎒 **Student Account**
- Access personal details and QR code.
- View individual course-wise attendance.
- Access overall attendance and attendance log.
- Check attendance for events and library.
- Download attendance report.

### 🛠️ **Device Process (IoT):**
1. Activate scanning mode with a switch press.
2. Scan QR code within 10 seconds.
3. Display the name and status on-screen post successful scanning.
4. Send notifications through the app.

### 🌐 **Server-Side Operations:**
- Generate new QR codes for students upon request (refresh every 30 seconds).
- Validate student permissions for events or classes.
- Record student data: in-time, out-time, event details, attendance duration, etc.
- Manage attendance records in a database.
- Maintain an Excel sheet for readability.

### 📱 **Mobile App Features:**
- Built on Flutter for cross-platform compatibility.
- Real-time notification services for reminders and attendance updates.
- Access to real-time data.
- Theme based on official branding and logo.

### 🤖 **IoT Interface (ESP32 based):**
- Recognizes and reads QR codes.
- Sends data to the server for verification.
- Provides real-time feedback to users through LED indicators and sound notifications.

### 📌 **Workflow:**
1. Students log into their accounts and display their QR codes.
2. The IoT device scans the QR code and sends it, along with its ID, to the server.
3. Server verifies the student details and updates the attendance.
4. Feedback is provided to the student through the device and mobile app notifications.