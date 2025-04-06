# Pokémon TCG Pocket Luck Calculator

An interactive, web-based calculator that lets you measure your luck in Pokémon TCG Pocket by comparing your actual card pulls to the expected pull rates. This educational project demonstrates advanced HTML, CSS, and JavaScript techniques—including local storage persistence, animated sprites, and responsive design—all wrapped in a retro, Pokémon-inspired aesthetic.

## Live Demo

Access the live version of the project here:  
[https://mikstrix.github.io](https://mikstrix.github.io)

## Features

- **Retro Pokémon Design:**  
  Uses the “Press Start 2P” font and a subtle repeating Pokéball background for a classic gaming vibe.

- **Interactive Inputs:**  
  Enter numbers for different card rarities (Crown Rares, Triple Stars, Double Stars, Single Stars, Quad Diamonds, God Packs, Shiny One Star, Shiny Two Star) along with the total packs opened and Shining Revelry packs. Inputs are validated in real time and saved via localStorage.

- **Dynamic Calculations:**  
  The calculator computes a "luck factor" for each card rarity by comparing your actual pulls to the expected pulls, then aggregates these into a final normalized score.

- **Animated Visuals:**  
  Enjoy animated floating Pokémon sprites and confetti effects that respond to your final luck score.

- **Responsive Layout:**  
  Optimized for both mobile and desktop screens for a smooth user experience.

- **Modular & Customizable:**  
  The code is organized so you can easily update pull rate percentages, tweak the luck factor formula, or swap in new rarity icons.

## Calculation Details

The luck score is derived by comparing your **Actual Pulls** against the **Expected Pulls** for each card rarity. Here’s how the calculation works:

1. **Expected Pull Rates:**  
   Each rarity has an assigned expected percentage that represents the chance of pulling that rarity in a booster pack. The values used in this calculator are as follows:
   - **Crown Rares:** 0.193%
   - **Triple Stars:** 1.12%
   - **Double Stars:** 2.55%
   - **Single Stars:** 12.7%
   - **Quad Diamonds:** 7.32%
   - **God Packs:** 0.05%
   - **Shiny One Star:** 2.857%
   - **Shiny Two Star:** 1.333%

2. **Expected Pulls Calculation:**  
   The expected number of pulls for a given rarity is calculated by multiplying its pull rate (as a decimal) by the total number of booster packs opened (or by the Shining Revelry packs count for shiny rarities).  
   For example:  
   - Expected Crown Rares = Packs Opened × 0.00193  
   - Expected Shiny One Star = Shining Revelry Packs Opened × 0.02857

3. **Luck Factor Calculation:**  
   For each rarity, the luck factor is computed using the formula:
Luck Factor (%) = (Actual Pulls / Expected Pulls) × 100 – 100

- A **0% luck factor** means you pulled exactly as expected.
- A **positive percentage** indicates you pulled more than expected.
- A **negative percentage** indicates you pulled fewer than expected.

4. **Normalization:**  
The individual luck factors are aggregated and then normalized to a 0–100 scale to yield your final overall luck score.

5. **Ignored Rarities:**  
Cards with a rarity lower than Quad Diamonds are assumed to be pulled 100% of the time and are therefore not tracked individually in the calculations.

## Installation & Usage

1. **Clone or Download the Repository:**  
Clone the repo or download the ZIP file.

2. **Open the Project:**  
Simply open `index.html` in your web browser—no server setup is required.

3. **Input Your Data:**  
Enter your card pull numbers and pack totals. The app validates your inputs and displays a detailed breakdown immediately.

4. **View Your Luck Score:**  
Click the **Submit** button to see your detailed luck score, complete with animated visual feedback.

## Code Overview

- **HTML:**  
Defines the structure of the calculator, including input forms, the results section, and informational details (e.g., "How It Works" and "How to Get Your Inputs").

- **CSS:**  
Provides the retro aesthetic, responsive layout, and animations (e.g., floating Pokémon, fade-in effects, and confetti animations).

- **JavaScript:**  
Handles input validation and persistence, calculates the luck factors using the formulas described above, dynamically updates the DOM with results, and manages animations. A mapping system for rarity icons is also included, which you can update with official or self-hosted image URLs as needed.

## Customization

- **Rarity Icons:**  
Update the URL mapping in the JavaScript to change the icons used for each card rarity. You might host your own images on GitHub Pages (or another service) and update the links accordingly.

- **Animations & Styles:**  
Modify the CSS keyframes (e.g., `floatAround`, `fadeInUp`, `slamIn`) to adjust the animation speed or style.

- **Calculation Logic:**  
The JavaScript is modular—feel free to change pull rates or tweak the luck factor formula to suit your needs.

## Contributing

Contributions, suggestions, and bug reports are welcome! Please open an issue or submit a pull request if you’d like to help improve the calculator or add new features.

## License

This project is intended for educational and non-commercial use. Please respect the trademarks and copyrights held by The Pokémon Company and its partners.