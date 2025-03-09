# Pokémon TCG Pocket Luck Calculator

A fun, web‑based calculator for Pokémon TCG Pocket that measures how “lucky” your pack pulls are based on in‑game probabilities. The app features a retro, Pokémon‑themed design with dynamic animations and confetti effects to celebrate your pulls (or commiserate when luck isn’t on your side).

---

## Features

- **Dynamic Luck Calculation:**  
  Compares the actual number of cards pulled against the expected pull rates for each rarity, then computes an overall "luck" score.

- **Animated Results:**  
  Enjoy animated effects – from confetti that fills the screen on high scores to a sad confetti effect on low scores, plus an animated Pokémon image that appears as your result.

- **Pokémon‑Inspired UI:**  
  Uses the retro "Press Start 2P" font, animated Pokéball icons in the title, and Pokémon‑themed messages throughout.

- **Responsive Design:**  
  Automatically adapts for smaller screens so it looks great on phones and tablets.

- **Local Storage:**  
  Saves your input values so you don’t have to re-enter data each time.

---

## Expected Pull Rates

- **Crown Rares:** 0.193%
- **Triple Stars:** 1.12%
- **Double Stars:** 2.55%
- **Single Stars:** 12.7%
- **Quadruple Diamonds:** 7.32%
- **Rare (God Pack):** 0.05%

> **Note:** Cards below Quadruple Diamonds are not tracked individually; they are assumed to be pulled at an average (100%) rate for every player.

---

## Usage

1. **Enter Your Pulls:**  
   Input the number of cards you pulled for each rarity and the number of packs opened.

2. **Submit & See Your Luck:**  
   Click the **Submit** button to calculate your overall luck score. The app will display a breakdown by rarity along with an animated Pokémon result and confetti effects based on your performance.

3. **How It Works:**  
   The “How It Works” section explains the calculation:
   - **Luck Factor (%)** is determined by comparing your actual pulls to the expected number, then scaling the result.
   - A 0% Luck Factor means you pulled exactly as expected. Positive values indicate extra pulls, while negative values indicate fewer pulls.
   - Each rarity is accompanied by a fun, Pokémon‑inspired message.

---

## License

This project is licensed under the [MIT License](LICENSE).

---

## Disclaimer

Pokémon, the Pokémon logo, Poké Balls, and all related icons and images are trademarks of Nintendo, The Pokémon Company, and their affiliates. This project uses these assets solely for personal, educational, and non-commercial purposes and is not endorsed, sponsored, or affiliated with Nintendo or The Pokémon Company.

---

## Attributions

- **Pokémon Sprites & Icons:**  
  Obtained from [PokeAPI](https://pokeapi.co/) and used in accordance with their usage guidelines.
- **Web Font:**  
  "Press Start 2P" is provided by [Google Fonts](https://fonts.google.com/).

---

Feel free to fork, contribute, or suggest improvements!
