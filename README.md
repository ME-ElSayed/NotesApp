# Notes App

A clean and simple Flutter notes application for creating, editing, organizing, and deleting notes with local persistent storage.

## Overview

Notes App is a Flutter project that demonstrates how to build a local offline notes experience using Hive for storage and Cubit/BLoC for state management.  
Users can add notes, choose a note color, update existing notes, and remove notes with swipe actions.

## Features

- Create new notes from a bottom sheet form
- Edit existing notes
- Delete notes with swipe confirmation
- Swipe to open the edit screen
- Assign custom colors to notes
- Persist notes locally using Hive
- Form validation for required fields
- Dark theme UI with custom Poppins font

## Tech Stack

- **Flutter**
- **Dart**
- **Hive**
- **flutter_bloc**
- **modal_progress_hud_nsn**

## Architecture

The project is structured around simple, reusable Flutter widgets and Cubits:

- **Hive** handles local storage
- **NotesCubit** loads all saved notes
- **AddNoteCubit** manages note creation states
- **NoteModel** defines the stored note data

## Project Structure

```bash
lib/
├── cuibts/
│   ├── add_note_cubit/
│   └── notes_cubit/
├── models/
│   ├── note_model.dart
│   └── note_model.g.dart
├── views/
│   ├── notes_view.dart
│   └── edit_note_view.dart
├── widgets/
├── constants.dart
├── main.dart
└── simple_bloc_observer.dart
