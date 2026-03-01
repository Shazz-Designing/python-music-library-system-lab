# Music Library System – OOP Lab

## Overview

This project implements a `Song` class using Object-Oriented Programming (OOP) principles in Python.

The class simulates a simplified music library system that:

- Creates song objects with a name, artist, and genre
- Tracks the total number of songs created
- Stores all unique artists
- Stores all unique genres
- Counts how many songs belong to each genre
- Counts how many songs each artist has

The project was implemented to satisfy the provided automated tests.

---

## Concepts Demonstrated

- Class creation and initialization
- Instance attributes
- Class attributes
- Shared state across instances
- Dictionary-based counting
- Set usage for uniqueness
- Automatic updates during object creation
- Test-driven development workflow

---

## Features

### Initialization

Each `Song` object:

- Stores `name`, `artist`, and `genre`
- Automatically increments the class-level `count`
- Updates:
  - `genres`
  - `artists`
  - `genre_count`
  - `artist_count`

---

## Class Attributes

The `Song` class maintains:

- `count` → total number of songs created
- `genres` → set of unique genres
- `artists` → set of unique artists
- `genre_count` → dictionary tracking number of songs per genre
- `artist_count` → dictionary tracking number of songs per artist

### Example Structure

```python
genre_count = {
    "Rap": 1,
    "Pop": 3,
    "Rock": 1
}

artist_count = {
    "Jay Z": 1,
    "Beyonce": 1,
    "Nirvana": 1,
    "Hall and Oates": 2
}
```

---

## How to Run

### 1. Install dependencies and activate the environment

```bash
pipenv install
pipenv shell
```

### 2. Run tests

```bash
pytest
```

---

## Test Results

All automated tests pass successfully:

```
6 passed, 0 failed
```

---

## Project Structure

```
lib/
└── song.py

lib/testing/
└── song_test.py
```