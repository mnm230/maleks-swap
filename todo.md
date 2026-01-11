# Maleks SWAP - Project TODO

## Midnight Aurora Redesign
- [x] Create new dark theme color palette
- [x] Implement animated aurora background
- [x] Design glassmorphism cards with blur effects
- [x] Add neon glow effects to interactive elements
- [x] Update typography to modern sans-serif (Space Grotesk)
- [x] Ensure high contrast and readability
- [x] Deploy new design to GitHub Pages

## Bug Fix: Live Rates
- [x] Investigate API response and error handling
- [x] Fix live rate update logic
- [x] Verify fix with local testing
- [x] Deploy fix to GitHub Pages

## Data Correction
- [x] Fetch current real-time stock prices (AAPL, GOOGL, MSFT, TSLA, AMZN)
- [x] Fetch current real-time exchange rates for verification
- [x] Update stock data in index.html with accurate values
- [x] Verify and update exchange rate logic/defaults
- [x] Deploy corrected version to GitHub Pages

## Fix: Stock Prices
- [x] Re-verify latest stock prices (AAPL, GOOGL, MSFT, TSLA, AMZN)
- [x] Remove `simulateFluctuations` logic for stocks to prevent data drift
- [x] Update stock data with verified static values
- [x] Deploy final fix to GitHub Pages

## Fix: Exchange Rates
- [x] Fetch authoritative exchange rates for USD to EUR, GBP, AED, PHP
- [x] Update base exchange rates in index.html
- [x] Verify live update logic handles rate normalization correctly
- [x] Deploy verified rates to GitHub Pages

## Verification: Rate Comparison
- [x] Fetch current exchange rates from Bloomberg/Reuters for USD to EUR, GBP, AED, PHP
- [x] Create comparison table between current app rates and new sources
- [x] Report findings to user

## Analysis: Volatility
- [x] Fetch 24-hour high/low and volatility data for EUR/USD and GBP/USD
- [x] Calculate if 0.0005 difference is within standard deviation
- [x] Report analysis to user

## Feature: Real-time Stocks
- [x] Research free stock APIs (Finnhub, Alpha Vantage, Yahoo Finance alternatives)
- [x] Select API with CORS support for frontend use
- [x] Implement API integration for AAPL, GOOGL, MSFT, TSLA, AMZN
- [x] Add new stocks: NVDA, META, NFLX
- [x] Deploy real-time stock updates to GitHub Pages

## Feature: Stock Search
- [x] Add search input and button to stock section UI
- [x] Style search bar to match Midnight Aurora theme
- [x] Implement search function to fetch new symbols from Finnhub
- [x] Add found stocks to the tracking list dynamically
- [x] Handle errors (invalid symbol, API limits)
- [x] Deploy search feature to GitHub Pages

## Redesign: Gen Z Neo-Brutalism
- [x] Define color palette (Acid Green, Hot Pink, Electric Blue, Black, White)
- [x] Replace glassmorphism with solid colors and thick black borders (3px)
- [x] Add hard shadows (box-shadow: 4px 4px 0px #000)
- [x] Update typography to bold, playful fonts
- [x] Add "pop" hover effects and interactions
- [ ] Deploy new design to GitHub Pages

## Fix: UX/UI Polish
- [x] Remove leftover gradients and text shadows from previous theme
- [x] Fix alignment issues in stock list and search bar
- [x] Ensure mobile responsiveness for Neo-Brutalist elements
- [x] Improve contrast for text on colored backgrounds
- [x] Fix any overflow issues caused by hard shadows
- [x] Deploy UX/UI fixes to GitHub Pages

## Redesign: Candy Pop
- [x] Define color palette (Lavender #8B5CF6, Mint #34D399, Coral #F472B6)
- [x] Replace hard borders with soft shadows (box-shadow: 0 10px 25px -5px rgba(0, 0, 0, 0.1))
- [x] Round corners to 24px for a friendly feel
- [x] Update typography to clean, modern sans-serif (Inter/Space Grotesk)
- [x] Add subtle gradients and glassmorphism back (but cleaner)
- [x] Deploy Candy Pop redesign to GitHub Pages

## Feature: Market Insights
- [x] Design "Market Insights" card with Candy Pop aesthetic
- [x] Add Exchange Rate Comparison table (Maleks vs Bloomberg)
- [x] Add Volatility Analysis summary
- [x] Style tables and text to match soft, rounded theme
- [x] Deploy Market Insights to GitHub Pages

## Fix: Candy Pop UX/UI
- [x] Fix mobile responsiveness for Market Insights table
- [x] Improve text contrast for accessibility (darker text on light backgrounds)
- [x] Adjust spacing in sidebar cards for better visual flow
- [x] Ensure all interactive elements have clear focus states
- [x] Deploy UX/UI fixes to GitHub Pages

## Redesign: Streamlined UX
- [x] Design tabbed navigation system (Swap, Stocks, Insights)
- [x] Implement single-card layout for focused interaction
- [x] Add scrolling stock ticker to header
- [ ] Enhance input fields for tactile, app-like feel
- [ ] Deploy Streamlined UX to GitHub Pages
