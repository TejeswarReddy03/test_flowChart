# My Flutter Application

This repository contains the source code for a Flutter application that provides a comprehensive interface for health-related services, including doctor consultations, prescriptions, and health advice.

## Features

- User Authentication with OTP
- Home screen with personalized content
- Bottom navigation bar for easy access to main sections
- Language selection, notifications, and profile management
- Health services, including prescriptions and doctor consultations
- Information and advice on eye health

## Flowchart

Below is the flowchart that illustrates the overall flow of the application:

```mermaid
graph TD;
    A[main.dart] -->|If logged in| B[bottomscreen.dart]
    A -->|Not logged in| C[loginpage.dart]
    C --> D[otppage.dart]
    D --> E[switchuser.dart]
    E --> B[bottomscreen.dart]

    B --> F[homescreen.dart]
    B --> G[servicepage.dart]
    B --> H[myfamily.dart]
    B --> I[settings.dart]
    B --> J[floating_icon]
    
    J --> K[vision.dart]

    F --> L[top navbar]
    L --> M[language_dialog.dart]
    L --> N[notification.dart]
    L --> O[myprofile.dart]

    F --> P[cardbox.dart]
    P --> Q[barcode.dart]
    
    F --> R[My Status]
    F --> S[My Actions]
    S --> T[prescription.dart]
    S --> U[treatment_advice.dart]
    S --> V[awareness.dart]
    S --> W[tips_to_reduce_eyestrain.dart]
    S --> X[facts_about_eye.dart]

    G --> Y[services.dart]
    Y --> T[prescription.dart]
    Y --> Z[connect_with_doctor.dart]
    Y --> AA[other_services.dart]

    I --> AB[viewprofile.dart]
    I --> N
    I --> AC[terms_and_conditions.dart]
    I --> AD[privacy_policy.dart]
    I --> AE[about.dart]
    I --> AF[logout.dart]
