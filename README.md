# 📚 ATLASS Attendance System

Welcome to the ATLASS Attendance System repository. This system allows for a seamless integration of attendance monitoring through QR code scanning. The system consists of three account levels: Admin, Teacher, and Student.

## 🚀 Features

### 1. 🧑‍💼 **Admin Account**
- ✨ Add new students.
- 🗓 Assign timetable to individual students or in batch.
- 🏫 Assign batches and sections to students in bulk.
- 📊 View attendance of a specific student.
- 📚 See attendance of a particular course.
- 📥 Download attendance reports in PDF format.

### 2. 🧑‍🏫 **Teacher Account**
- 📜 View students assigned to them.
- 📌 View and edit class timings.
- 📅 View attendance of each student.
- 💾 Download attendance reports.

### 3. 🧑‍🎓 **Student Account**
- 🤳 View personal details and QR code.
- 📉 View attendance course-wise and overall.
- 🗂 View timetable.
- 📖 View attendance log.
- 📚 View attendance for various events and library sessions.
- 📤 Download attendance reports.

### 🖥 **Device Process (User Side)**
- 🔘 Press switch to activate scanning mode.
- 📸 Scan QR code within a 10-second timeframe.
- 🎉 If scanned correctly, the student's name and status will appear on-screen.
- 📳 Receive a mobile app notification about the scan status.

### 💡 **Back-end Process (Device)**
- 🔍 Initiate QR recognition upon switch activation.
- 🎫 Upon QR recognition, retrieve the key and display the name on the screen.
- 🌐 Send the unique student identification (SAP) and location to the server.
- 📊 Organize the data received from the device.
- 🔄 Update student records and dispatch a notification.

### 📱 **Operational Flow**
Students, upon logging into their account, will present their QR code to the camera. If the scanner successfully detects the QR, a positive response is returned. If not, the scanner will indicate an error and retry until successful.

### 🖧 **Server Functionality**
- 🔁 Generates a fresh QR code for each student every 30 seconds (on request).
- ✅ Validates if a student is permitted to attend an event or class. Sends an error if not.
- 📄 Stores details like student in-time, out-time, event/class details, total attendance, and event/class population.
- 📑 Manages an Excel sheet for enhanced readability.

## 📜 Setup and Usage
1. **Clone the Repository**
    ```bash
    git clone [repository-url]
    ```

2. **Navigate to the Repository**
    ```bash
    cd path-to-repo
    ```

3. **Run the Application**
    Follow the setup instructions in the `INSTALLATION.md` file.

## 💡 Contribution
Feel free to fork this repository, make changes, and submit pull requests. For substantial changes, please open an issue first.

## 📜 License
MIT License. Check out the `LICENSE` file for more information.

