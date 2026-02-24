# BetterRest - ML-Powered Sleep Calculator 🌙☕️

## 📌 Project Overview
**BetterRest** is an intelligent iOS application that helps users calculate their optimal bedtime. Instead of relying on static rules, this app uses a trained **Machine Learning (Core ML)** model to predict exactly when you should go to sleep based on your desired wake-up time, preferred sleep duration, and daily caffeine intake. 

## 🌟 Key Features
* **Machine Learning Predictions:** Integrates a custom `.mlmodel` trained on sleep data to output accurate, personalized bedtime recommendations.
* **Intuitive User Input:** Utilizes SwiftUI `Form`, `DatePicker`, and `Stepper` components to seamlessly gather user preferences.
* **Smart Date & Time Handling:** Calculates and formats complex `Date` and `DateComponents` behind the scenes to ensure accurate time math.
* **Instant Feedback:** Displays the recommended bedtime immediately via an interactive pop-up alert.

## 🛠️ Technologies Used
* **Swift 5 & SwiftUI:** For a declarative, state-driven user interface.
* **Core ML:** Apple's machine learning framework, used to load and query the trained regression model (`SleepCalculator.mlmodel`).
* **Create ML:** (Used to initially train the tabular regression model using a dataset of sleep patterns).

## 🧠 Developer Highlights
This project demonstrates my ability to step beyond basic UI and integrate advanced native frameworks:
* **Core ML Integration:** Successfully imported a compiled machine learning model and safely handled prediction errors using `do-catch` blocks.
* **Advanced State Management:** Used `@State` property wrappers to bind user inputs directly to the UI, ensuring the model always evaluates the most up-to-date data.
* **Time Math:** Demonstrated proficiency with Apple's `Calendar` and `DateComponents` APIs to convert user-selected times into seconds, run the ML prediction, and convert the output back into a human-readable `Date` format.

## 🚀 How to Run Locally
1. Clone this repository to your local machine.
2. Open `BetterRest.xcodeproj` in Xcode.
3. Ensure the `SleepCalculator.mlmodel` is securely in the project navigator.
4. Select a simulator (e.g., iPhone 15 Pro) and hit **Run (Cmd + R)**.
