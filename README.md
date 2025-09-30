🚀 Hybrid Integration Challenge: Native Kotlin to Flutter
Project Goal
The primary objective of this challenge is to assess your ability to implement a robust hybrid mobile application architecture. You will be tasked with integrating and managing a persistent Flutter Engine within a Native Android (Kotlin) application, demonstrating lifecycle management and seamless native-to-Flutter navigation using specific routes.

Prerequisites
To successfully complete this project, please ensure you have the following tools and knowledge:
Development Environment: Android Studio (Dolphin or later) installed.
SDKs: Flutter SDK (v3.19 or later) installed and configured for your environment.
Language Proficiency: Strong knowledge of Kotlin (minimum v1.8).
Framework Familiarity: Experience working with the Flutter FlutterEngine and FlutterActivity classes.
🛠️ Task Description (Deliverables)
You will be creating or modifying an Android shell project and an associated basic Flutter module.

Phase 1: Engine Caching and Initialization
Initialize the Flutter Engine: As soon as the native application starts, modify the Android application logic (e.g., in a custom Application class) to eagerly initialize and cache a single instance of the FlutterEngine.
Engine Name: The cached engine instance MUST be named my_cached_engine.
Phase 2: UI and Route Setup
Native UI: Create a single native Kotlin Activity (the main landing page) that hosts two distinct Button elements.
Flutter Module: Create a simple Flutter module containing two separate screens/widgets:
HomePage: Maps to the default route (/).
DetailPage: Maps to the named route (/detail).
Phase 3: Native-to-Flutter Navigation
The two buttons on the native Kotlin activity must launch the Flutter environment using the cached engine (my_cached_engine), navigating directly to the specified Flutter route.

Button Label

Action Required

Flutter Route Target

Purpose

Open Home

Launch Flutter Activity

/ (HomePage)

Test default route launch.

Open Detail

Launch Flutter Activity

/detail (DetailPage)

Test named route launch.

Key Requirement: The solution must reuse the pre-initialized and cached my_cached_engine for both navigation actions to avoid engine recreation.

提交 Submission Guidelines
Repository Setup: Fork this challenge repository or create a new one to host your solution.
Commit Quality: Maintain a clean, logical, and descriptive commit history detailing the steps taken.
Final State: Ensure the final, runnable code is pushed to the main branch (main or master).
Instructions: Include clear instructions in the README.md on how to run and test the application from a clean checkout (e.g., "how to link the Flutter module," "build steps").
📊 Evaluation Criteria
Your solution will be thoroughly assessed based on the following weighted criteria:

Criteria

Weight

Focus Area

Engine Caching

40%

Correct initialization of the my_cached_engine on startup and its subsequent reuse by both native buttons.

Correct Routing

30%

Successful launch of the Flutter environment to the default route (/) and the specific named route (/detail) via the native buttons.

Code Quality

20%

Readability, adherence to Kotlin and Dart best practices, clear separation of platform-specific and framework logic, and modern API usage.

Documentation

10%

Clarity of inline comments for complex logic and thoroughness of submission/running instructions.

Good luck! We look forward to seeing how you handle this modern mobile development scenario.
