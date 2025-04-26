# Astro-Musical Forecaster 🎵✨🪐

**An exploratory project correlating personal Spotify listening history with daily astrological transits to forecast potential future musical preferences.**

---

## Overview

This project delves into a creative and experimental intersection: music listening habits and astrology. The core idea is to explore whether patterns exist between a user's detailed Spotify listening history (moods, genres, energy levels reflected in music choices) and the specific astrological planetary transits occurring relative to their birth chart on those listening days.

Using Python, the `swisseph` library for precise astronomical calculations, and the `spotipy` library (potentially) for enriching track data, this system processes historical listening data alongside calculated daily transits. It then attempts to build a simple predictive model to forecast characteristics (like average audio features, e.g., valence or energy) of music a user might gravitate towards on future dates based on upcoming transit patterns.

**Disclaimer:** This is a highly experimental proof-of-concept built primarily as a technical challenge and creative exploration. It aims to showcase skills in data processing, API integration, time-series concepts, astrological calculation programming, and machine learning workflow implementation. It does **not** aim to scientifically validate astrological claims, and any correlations found are likely coincidental or influenced by other factors.

---

## Features (Planned / Implemented)

*   **Spotify History Ingestion:** Parses detailed `StreamingHistoryX.json` files provided by the user.
*   **Natal Chart Calculation:** Computes planetary positions at the time of birth using `swisseph`.
*   **Daily Transit & Aspect Calculation:** Determines daily positions of transiting planets and calculates significant aspects (conjunctions, squares, trines, etc.) relative to the natal chart for the duration of the listening history.
*   **Data Aggregation:** Summarizes daily listening patterns (e.g., average audio features, listening duration).
*   **Feature Engineering:** Converts astrological events (active aspects, planet signs/degrees) and listening history into numerical features.
*   **Exploratory Data Analysis (EDA):** Visualizes listening trends and explores potential visual correlations between music choices and specific astrological events.
*   **(Experimental) Predictive Modeling:** Trains a simple ML model to predict future listening characteristics based on upcoming transits.
*   **Local API (FastAPI):** Provides simple endpoints to input birth data and get predictions for a future date.

---
