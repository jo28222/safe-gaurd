# SafeGaurd – Women Safety & Cyber Protection App

## Overview

**SafeGaurd** is a mobile safety application built using **Flutter** and **Android Native integration**.
The goal of this project is to provide a **fast emergency response system**, **anonymous harassment reporting**, and **phishing detection** to protect women from both **physical and cyber threats**.

The application allows users to quickly send emergency alerts, report harassment anonymously, and detect suspicious or phishing messages.

---

# Features

## 1️ Emergency SOS System

The SOS system allows users to quickly request help in emergency situations.

### How it works

* User presses the **power button three times**
* The app automatically triggers an **SOS alert**
* The app collects the **user’s live location**
* An **SMS message containing a Google Maps location link** is sent to a predefined contact

### Message Example

!!EMERGENCY ALERT
I need help immediately.

My Live Location
https://www.google.com/maps?q=LATITUDE,LONGITUDE

### Technologies Used

* Flutter UI
* Android Native (Kotlin)
* MethodChannel communication
* Geolocator for location tracking
* Android SMS manager

---

# 2️ Anonymous Harassment Reporting Platform

This feature allows victims to **report harassment safely and anonymously**.

### Features

Users can submit:

* Written incident description
* Evidence text
* Voice recordings

### Privacy

* No personal identity is stored
* Each report receives an **anonymous Case ID**
* Victims can track their reports using **My Cases**

### Intended Real-World Use

In the real system the reports can be shared with:

* Verified psychiatrists
* Mental health advisors
* Women support groups
* Legal assistance teams

---

# 3️ Phishing Detection System

This module allows users to analyze suspicious messages or links.

### Workflow

1. User pastes a suspicious message or link
2. The system performs **risk analysis**
3. A **threat level** is generated

### Risk Levels

* Low Risk
* Medium Risk
* High Risk

### Demo Mode

In this demo version, results are **sent via SMS** to a test number.

### Real System

The report can be forwarded to:

* Cyber Crime Department
* Police Cyber Cell
* Threat intelligence systems

---

# 4️ Threat Analytics

The application includes a **basic threat analytics module**.

This module tracks:

* Number of harassment reports
* Phishing incidents detected
* SOS alerts triggered

In a real deployment this data can help authorities understand **crime patterns and risk zones**.

---

# System Architecture

Flutter (Frontend UI)
↓
Android Native (SOS trigger & SMS)
↓
Local Processing / Demo SMS System
↓
Authorities / Support Systems (Real implementation)

---

# Technology Stack

Frontend

* Flutter
* Dart

Mobile Integration

* Kotlin (Android Native)

Libraries Used

* geolocator
* permission_handler
* path_provider
* record

Communication

* Flutter MethodChannel

---

# Project Structure

lib/

main.dart → Main application logic
screens/
    report_harassment.dart → Anonymous reporting system
    my_cases_screen.dart → View submitted cases

android/
    MainActivity.kt → Native SOS trigger and SMS system

pubspec.yaml → Dependency configuration

---

# Installation

### Step 1 – Install Flutter

Install Flutter from
https://flutter.dev/docs/get-started/install

Verify installation:

flutter doctor

---

### Step 2 – Clone or Download the Project

Extract the project folder.

---

### Step 3 – Install Dependencies

Run:

flutter pub get

---

### Step 4 – Run the App

Connect an **Android device** and run:

flutter run

---

# Permissions Required

The application requires the following Android permissions:

* SMS permission
* Location permission
* Microphone permission
* Storage permission

These permissions are required for:

SOS alerts
Location sharing
Voice evidence recording

---

# Usage Guide

### Sending SOS

1. Press **Send SOS button**
2. Or press **Power button 3 times**
3. Emergency SMS will be sent automatically.

---

### Reporting Harassment

1. Open **Report Harassment**
2. Write incident description
3. Add voice evidence (optional)
4. Submit anonymously
5. Case ID will be generated

---

### Viewing Submitted Reports

1. Open **My Cases**
2. View previously submitted anonymous reports

---

### Phishing Detection

1. Enter suspicious message or link
2. Click **Analyze Threat**
3. Risk level will be shown

---

# Future Improvements

* Backend server integration
* AI phishing detection model
* Police emergency API integration
* Secure encrypted report database
* Real-time authority alerts
* Live emergency tracking system

---

# Purpose of the Project

This project aims to demonstrate how **mobile technology can improve women's safety** by providing:

* Faster emergency response
* Anonymous reporting channels
* Cybercrime awareness tools
* Mental health support pathways

---

# Developer

Project Name: **SafeGaurd – Women Safety System**
Developed using Flutter and Android Native Integration.

---

# License

This project is developed for **educational and demonstration purposes**.
