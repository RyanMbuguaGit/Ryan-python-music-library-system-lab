# Music Library System - Song Class

## Description

This project implements a `Song` class in Python that models an individual song and tracks statistics across all songs created. It was built as part of a lab on inheritance, class attributes, and class methods.

## Song Class

Each `Song` instance has:
- `name` — the song's title
- `artist` — the song's artist
- `genre` — the song's genre

The class also tracks global statistics across every song created, using class attributes:
- `count` — total number of songs created
- `genres` — list of all unique genres seen
- `artists` — list of all unique artists seen
- `genre_count` — dict mapping each genre to how many songs belong to it (e.g. `{"Rap": 5, "Rock": 1}`)
- `artist_count` — dict mapping each artist to how many songs they have (e.g. `{"Beyonce": 17, "Jay-Z": 40}`)

Each time a new `Song` is instantiated, class methods automatically update these class attributes:
- `add_song_to_count`
- `add_to_genres`
- `add_to_artists`
- `add_to_genre_count`
- `add_to_artist_count`

## Testing

All tests pass:
6 passed in 0.29s
## Setup

pip install pytest
cd lib
pytest testing/song_test.py -v

---

## Original Lab Instructions

*(kept below for reference)*