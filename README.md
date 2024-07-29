# QR Code Scanner App

This project is a QR Code Scanner application built using Jetpack Compose and Google's ML Kit. The app utilizes CameraX to access the device's camera, scan QR codes, and display the decoded information on the screen.

## Table of Contents

- [Features](#features)
- [Screenshots](#screenshots)
- [Architecture](#architecture)
- [Technologies Used](#technologies-used)
- [Setup and Installation](#setup-and-installation)
- [Usage](#usage)
- [Contributing](#contributing)
- [License](#license)

## Features

- **Real-time QR Code Scanning:** Uses CameraX and ML Kit for efficient scanning of QR codes.
- **Jetpack Compose UI:** Modern UI with Compose, offering a smooth and responsive user experience.
- **Permission Handling:** Uses Accompanist for handling runtime permissions gracefully.
- **Display Results:** Shows decoded QR code data in a user-friendly format.

## Screenshots

Here are some screenshots of the application in action:

| Scanning QR Code | Displaying QR Data |
|------------------|--------------------|
| ![Scanning](screenshots/scanning.png) | ![Displaying QR Data](screenshots/displaying_qr_data.png) |

## Architecture

The project follows a straightforward architecture using Jetpack Compose and CameraX:

- **MainActivity:** The main entry point, handling camera initialization and managing the UI.
- **Composable Functions:** Individual composable functions are used to build the UI, such as `CameraPreview`, `QRCodeResult`, and `CameraPermission`.
- **QRCodeAnalyzer:** This class processes each camera frame to detect and decode QR codes using ML Kit.
- **State Management:** Uses Compose's `remember` and `mutableStateOf` for managing UI state and QR code results.

## Technologies Used

- [**Jetpack Compose**](https://developer.android.com/jetpack/compose): For building the UI in a declarative manner.
- [**CameraX**](https://developer.android.com/training/camerax): To access and control the camera.
- [**ML Kit**](https://developers.google.com/ml-kit): For barcode scanning and QR code detection.
- [**Accompanist**](https://github.com/google/accompanist): For managing permissions in Compose.
- [**Kotlin**](https://kotlinlang.org/): The programming language used for building the application.


### Installation Steps

1. **Clone the Repository:**

   ```bash
   git clone https://github.com/shafaque/ComposeScanner.git
   cd ComposeScanner


