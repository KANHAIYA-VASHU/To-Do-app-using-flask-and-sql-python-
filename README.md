# Todo List Application

A simple and elegant Todo List application built with Flask and SQLite.

## Features

- Add new tasks
- Mark tasks as complete/incomplete
- Delete tasks
- Responsive design
- Persistent storage using SQLite database

## Installation

1. Install the required dependencies:
```
pip install -r requirements.txt
```

2. Run the application:
```
python app.py
```

3. Open your web browser and navigate to `http://localhost:5000`

## Usage

- To add a task: Type your task in the input field and click "Add Task"
- To mark a task as complete: Click the "Complete" button next to the task
- To delete a task: Click the "Delete" button next to the task

## Technologies Used



Developing an Android Battery Saver app is a great project idea, especially for a final-year computer science student. It allows you to tackle various advanced concepts, from Android app development and power management to potentially integrating machine learning to predict battery drain. Here’s how you can approach this project:

Project Overview:
The Android Battery Saver app will monitor and optimize battery consumption by managing various device features and processes. It will allow users to have control over various settings such as background apps, Wi-Fi, Bluetooth, screen brightness, GPS, etc. Advanced features can include AI/ML to predict battery usage and give personalized tips.

Project Breakdown:
1. Core Features to Implement:
These features aim to optimize the user's battery consumption without compromising usability.

Battery Usage Monitoring:

Track the battery percentage and health in real-time.
Monitor apps and processes using excessive battery.
Use Android’s BatteryManager API to get battery status.
Background Processes Control:

Identify and stop high battery-consuming background apps or processes using Android’s UsageStatsManager and JobScheduler APIs.
Screen Brightness Control:

Dynamically adjust screen brightness based on battery level or user preferences. Use Settings.System.putInt for managing screen brightness.
Connectivity Management (Wi-Fi/Bluetooth/GPS):

Turn off Wi-Fi, Bluetooth, or GPS when they are not needed, saving battery. For instance, use BluetoothAdapter and WifiManager for Bluetooth and Wi-Fi management.
Optionally, offer the user a setting to toggle "Do not disturb" or set automatic connectivity rules based on battery level.
Power-Saving Modes:

Provide predefined battery-saving profiles (e.g., Power Saver, Ultra Power Saver).
Use Android's PowerManager to implement CPU sleeping states and screen timeout adjustments.
2. Advanced Features (Optional but Highly Recommended):
AI-based Battery Drain Prediction:

Use machine learning algorithms (e.g., regression models) to predict future battery drain based on current usage patterns.
Collect historical data about the battery level, app usage, and device states, and use it to train a model that can predict battery consumption in real time.
Personalized Recommendations:

Based on the user’s habits (e.g., specific app usage patterns), suggest personalized battery optimization tips. For example, if the user often leaves GPS on, suggest turning it off when not in use.

The recommendation system could be powered by machine learning models like decision trees or neural networks to offer customized suggestions.

3. User Interface (UI):
Simple and User-Friendly UI:

The app should have a clean, intuitive UI that allows users to easily monitor battery usage and activate power-saving modes.
Provide clear information about which apps are consuming the most battery, with an option to stop them directly from the app.
Real-Time Updates:

Display real-time updates of battery health, percentage, and active power-saving modes.
4. Battery Saver Modes:
Offer different levels of battery-saving modes, such as:

Power Saver Mode: Decreases background data usage, reduces screen brightness, and adjusts sync settings.
Ultra Power Saver Mode: Disables unnecessary features (e.g., Wi-Fi, Bluetooth, GPS), limits background apps, and dims the screen.
5. Notifications & Alerts:
Push notifications to alert the user when the battery reaches a critical level, or when they can benefit from activating a power-saving mode.
Alerts when apps or services consume unusually high power.
Technologies/Tools You’ll Need:
Android Development (Java/Kotlin):

Use Android Studio as your IDE and either Java or Kotlin for app development.
Familiarize yourself with the Android SDK, especially APIs related to power management and device state.
Battery Management APIs:

Use the BatteryManager class to monitor battery status.
Explore the JobScheduler API for managing background tasks and app activities that could impact battery consumption.
Machine Learning (Optional, Advanced Feature):

Use TensorFlow Lite or other libraries for building and deploying a machine learning model.
You can start with a simple regression model or decision tree to predict battery usage based on historical data.
Performance Optimization Techniques:

Implement Lazy Loading for background tasks to improve performance.
Optimize app startup time and memory usage, and ensure minimal impact on battery life when the app is running.
Implementation Plan:
Phase 1: Setup and Basic Features

Start with setting up the Android project in Android Studio.
Implement real-time battery percentage tracking.
Create a basic UI to display battery status and app usage data.
Phase 2: Power Management Features

Implement features to control screen brightness and Wi-Fi/Bluetooth.
Integrate background task management and provide options to stop high battery-draining processes.
Phase 3: Power Saving Modes

Implement predefined battery-saving modes with toggle buttons for user control.
Use Android’s PowerManager and WifiManager to disable unnecessary services.
Phase 4: Advanced Features (Optional)

Implement machine learning for battery drain prediction.
Develop a recommendation engine for personalized suggestions.
Phase 5: Testing and Optimization

Test the app on various devices to check its efficiency and impact on battery usage.
Optimize any memory or CPU-heavy operations to minimize power drain.
Challenges and Considerations:
Device Variability: Android devices vary in terms of hardware, OS versions, and power management features. Make sure to test across different devices and handle edge cases.
Battery Health: In some cases, users may not understand that the battery’s degradation is not related to app usage but to the natural aging of the battery itself. Clear messaging within the app can help mitigate confusion.
Permissions: The app will need to request several permissions to access Wi-Fi, Bluetooth, GPS, and background app usage. Ensure you handle these properly, considering privacy concerns.
Conclusion:
By building a Battery Saver app, you’ll be able to showcase your understanding of Android development, power management, and even delve into machine learning for predictions. It's a practical project that not only allows you to develop useful features but also solves a real-world problem for users—helping them prolong the battery life of their Android devices.





- Flask
- SQLAlchemy
- SQLite
- HTML/CSS
