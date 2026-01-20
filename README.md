Wi‑Fi Indoor Positioning System (RSSI Fingerprinting)
📌 Overview

This project is a Wi‑Fi–based indoor positioning website that determines a user’s location using RSSI fingerprinting.
The system compares user‑provided RSSI values against a pre‑built fingerprint database and predicts the most likely indoor location.
Unlike GPS, which performs poorly indoors, this system leverages existing Wi‑Fi access points for localization.

⚙️ How It Works

Offline Phase (Fingerprinting)
RSSI values are collected from multiple Wi‑Fi access points at known locations.
These RSSI vectors are stored in a fingerprint database along with location labels.

Online Phase (Localization)
The user runs the website and pastes the current RSSI values.
The system compares the input RSSI vector with the fingerprint database.
The closest match is selected and the corresponding location is displayed.

🧠 Localization Technique

Method: Wi‑Fi Fingerprinting
Matching Algorithm: Nearest Neighbor / k‑Nearest Neighbor (RSSI similarity based)
Distance Metric: Euclidean distance between RSSI vectors


Open the website in a browser
http://localhost:8000
Paste the json files
Click Locate to view the predicted location


(Format may vary depending on implementation)

🎯 Features

Indoor localization using Wi‑Fi signals
Simple and user‑friendly web interface
Fingerprint‑based positioning
Works without GPS

Lightweight and easy to deploy

⚠️ Limitations

RSSI values fluctuate due to obstacles and interference
Accuracy depends on fingerprint database quality
Manual RSSI input (no automatic scan)
Environmental changes may affect results

🔮 Future Enhancements

Automatic RSSI capture
Improved accuracy using weighted k‑NN
Real‑time positioning

Floor‑map visualization

Mobile device integration
