# Chrome Extension for Phishing Website Detection

## Overview

This Chrome extension is designed to detect phishing websites, ensuring user safety while browsing. It leverages a machine learning model implemented in Python (using a Multilayer Perceptron algorithm) to analyze websites for phishing indicators. The backend, built with Node.js, facilitates seamless communication between the extension and the detection system.

## Features

- **Phishing Website Detection:** Uses a trained MLP (Multilayer Perceptron) model to identify phishing threats.
- **Backend Integration:** Handles API requests and connects the Chrome extension with the detection model.
- **Real-Time Analysis:** Detects and flags phishing websites during user navigation.
- **Simple Chrome Extension Interface:** Easy to install and use for non-technical users.

## Technologies Used

- **Frontend:** Chrome Extension (HTML, JavaScript, CSS)
- **Backend:** Node.js
- **Machine Learning:** Python, MLP algorithm
- **Communication:** RESTful API for backend-extension interaction

## Installation and Usage

### Prerequisites

1. **Node.js** installed on your system.
2. **Python 3.x** installed, along with necessary libraries.
3. **Google Chrome** browser.

### Setup Steps

#### 1. Clone the Repository

```bash
git clone https://github.com/vivekPatil45/Malicious-Website-Detection-Web-Extenstion.git
cd Malicious-Website-Detection-Web-Extenstion
```

#### 2. Install Dependencies

##### Backend

Navigate to the `backend` directory and Install the required Node.js packages:

   ```bash
   cd backend
   npm install
   ```

Navigate to the Python model directory (if present) and install the required libraries:
 ```bash
cd ../model
pip install -r requirements.txt
```

#### 3. Start the Backend Server
Run the Node.js server:

```bash
cd ../backend
node server.js
```

#### 4. Load the Chrome Extension

1. Open the Google Chrome browser.
2. Go to `chrome://extensions` in the address bar.
3. Enable **Developer Mode** (toggle the switch at the top-right corner).
4. Click on **Load unpacked**.
5. Browse to the `extension` folder in the project directory and select it.
6. The extension will now appear in the list of installed extensions and be ready to use.

#### 5. Use the Extension

1. Open the Google Chrome browser.
2. Navigate to any website.
3. The extension will automatically analyze the website for phishing indicators.
4. If a phishing threat is detected, a warning message will be displayed.


## Customization

- **Machine Learning Model:** 
  - Replace or retrain the model located in the `model` folder to improve detection accuracy.
  
- **Backend Configuration:** 
  - Modify the `server.js` file in the `backend` folder to add new features or customize the API responses.

- **Frontend (Chrome Extension):** 
  - Update the `popup.html` and `popup.js` files in the `extension` folder to enhance the user interface or functionality.
