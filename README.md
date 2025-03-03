# Pokémon TCG Pocket Luck Calculator

This is a fun, Pokémon-themed luck calculator for Pokémon TCG Pocket! It lets you input the number of cards you pulled for each rarity (e.g., Crown Rares, Triple Stars, etc.) along with the number of packs opened, then calculates:

- A **Raw Luck Score** for each rarity: `(Actual Pulled ÷ Expected) × 100`
- An **Overall Luck Score** using an original summation and normalization method.
- A matching overall description and a Pokémon image based on your final score.
- Fun animations such as confetti for high scores and "sad confetti" for very low scores.

## Features

- **Responsive Input Layout:** Rarity inputs are arranged in compact cards in a grid, with a separate card for the number of packs opened.
- **Validation:** Ensures the total number of cards pulled doesn't exceed the maximum possible (assuming 5 cards per pack).
- **Themed Descriptions:** Unique Pokémon-themed messages for each rarity and overall score range.
- **Animations:** Pulse or shake animation on the overall score box, with confetti effects based on your luck.
- **Pokémon Image:** Displays an image (sourced from the official PokeAPI sprites) corresponding to your overall luck.

## How to Use

1. Open the `index.html` file in your browser.
2. Enter the number of cards you pulled for each rarity.
3. Enter the number of packs opened.
4. Click the **Submit** button.
5. The calculator will display your overall luck score, a detailed breakdown, and a Pokémon image and message representing your performance.

## Customization

- **Maximum Cards per Pack:** The calculator assumes a maximum of 5 cards per pack. Adjust this in the JavaScript if needed.
- **Image URLs:** The Pokémon images are loaded from the official PokeAPI sprites. You can update these URLs to your preferred images.
- **Descriptions & Ranges:** Both per-rarity and overall descriptions are customizable via arrays in the JavaScript.

## License

This project is licensed under the MIT License.
