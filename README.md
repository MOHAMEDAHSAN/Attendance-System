<img width="1402" height="507" alt="image" src="https://github.com/user-attachments/assets/c46adc54-9611-4d77-b8e5-72e39f6b247c" /># Face Recognition Based Attendance System

This is a Python-based application that uses OpenCV and Tkinter to create a complete system for registering users, training a face recognizer, and marking attendance automatically.

---

## 📋 Features

* **Register New Users:** Easily add new students/users by entering their ID and Name.
* **Capture Face Data:** Takes 100 images of the user's face to create a robust dataset.
* **Train Recognizer:** Trains a LBPH (Local Binary Patterns Histograms) Face Recognizer on the collected face data and saves the profile.
* **Take Attendance:** Opens the camera, detects faces, and compares them against the trained model to mark attendance in real-time.
* **Log Attendance:** Automatically saves attendance records in a CSV file for the current date.
* **View Attendance:** Displays the day's attendance log directly in the application window.
* **Password Protection:** Secures the "Save Profile" (training) function with a password.

---

## 🛠️ Installation & Setup

### 1. Prerequisites

This project relies on several Python libraries. You can install them all using `pip`:

pip install tk-tools pip install opencv-contrib-python pip install datetime pip install pytest-shutil pip install python-csv pip install numpy pip install pillow pip install pandas pip install times


**Important:** You must use `opencv-contrib-python` and not the standard `opencv-python` to get the `face` module.

### 2. Haar Cascade File

This program requires the `haarcascade_frontalface_default.xml` file to detect faces. You must download this file and place it in the same directory as `main.py`.

You can find this file in the [OpenCV GitHub repository](https://github.com/opencv/opencv/blob/master/data/haarcascades/haarcascade_frontalface_default.xml).

---

## 🚀 How to Use

1.  **Run the Application:**
    ```
    python main.py
    ```

2.  **Register a New User:**
    * In the "For New Registrations" section, enter the user's **ID** and **Name**.
    * Click the **"Take Images"** button. A camera window will open. Hold still until 100 images are captured.
    * Repeat for all new users.

3.  **Train the Model:**
    * After taking images, click the **"Save Profile"** button.
    * You will be prompted to set or enter a password.
    * The system will train on all the images in the `TrainingImage` folder and save the model.

4.  **Take Attendance:**
    * In the "For Already Registered" section, click the **"Take Attendance"** button.
    * The camera will open and begin recognizing faces.
    * Recognized individuals will be marked present, and their attendance will be logged and displayed in the table.
    * Press **'q'** to quit the attendance window.

---

## Diagrams:

<img width="1611" height="408" alt="image" src="https://github.com/user-attachments/assets/0adfba85-7223-4126-b24b-8b8e2df2c3e3" />

<img width="1555" height="483" alt="image" src="https://github.com/user-attachments/assets/371daed6-784a-45ae-b652-ca3b683010c5" />

<img width="1402" height="507" alt="image" src="https://github.com/user-attachments/assets/16ddabee-623c-4494-9754-e8d2216caebe" />



## 🧑‍💻 Author

* **Name:** Ponguru Aasrith Saira
* **Register Number:** 212223240116
* **Department:** AIML
