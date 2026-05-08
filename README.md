# Flutter Flashcard Quiz App

A quiz app built with Flutter & Dart, following [Academind's Flutter & Dart - The Complete Guide](https://www.udemy.com/course/learn-flutter-dart-to-build-ios-android-apps/) on Udemy.

## Features

- Answer multiple-choice questions with shuffled answers
- Track selected answers and display results summary
- Show correct/wrong answer count
- Restart quiz to play again
- Multi-screen navigation with conditional rendering

## What I Learned

- **Conditional Rendering** — switching screens with ternary expressions and state variables
- **Lifting State Up** — sharing state between sibling widgets via a common parent
- **Passing Functions as Values** — `void Function()` type, function pointers as widget arguments
- **Widget Lifecycle** — `initState()`, `build()`, `dispose()`
- **Data Model** — custom class (`QuizQuestion`) with getter for shuffled answers
- **map() + Spread Operator** — dynamically generating widget lists from data
- **Maps** — `Map<String, Object>` for key-value summary data
- **Other** — `OutlinedButton.icon()`, `Opacity`, `SingleChildScrollView`, `Expanded`, `Column` + `Row`

## Project Structure

```
lib/
├── main.dart               # App entry point
├── quiz.dart               # Main Quiz widget (Stateful, manages screens)
├── start_screen.dart       # Start screen with "Start Quiz" button
├── questions_screen.dart   # Displays questions + answer buttons
├── results_screen.dart     # Shows score summary
├── answer_button.dart      # Reusable answer button widget (Stateless)
├── questions_summary/
│   ├── questions_summary.dart
│   └── summary_item.dart
├── models/
│   └── quiz_question.dart  # QuizQuestion data model
└── data/
    └── questions.dart      # List of quiz questions
```

## Getting Started

### Prerequisites

- [Flutter SDK](https://docs.flutter.dev/get-started/install)
- An emulator or physical device

### Run

```bash
git clone https://github.com/NetKanet/flutter-flashcard-quiz-app.git
cd flutter-flashcard-quiz-app
flutter pub get
flutter run
```

## Screenshots

<!-- Add screenshots here -->

## Credits

- [Flutter & Dart - The Complete Guide](https://www.udemy.com/course/learn-flutter-dart-to-build-ios-android-apps/) by Maximilian Schwarzmuller (Academind)
- Section 3 — Flutter & Dart Basics II (Quiz App)
