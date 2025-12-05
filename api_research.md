# Live Exchange Rate API Research

## Date: December 5, 2025

### APIs Found:

#### 1. **ExchangeRate-API** (https://www.exchangerate-api.com/)
- **Type**: Fiat currency exchange rates
- **Free Tier**: Yes - requires API key but free plan available
- **Coverage**: 165 currencies (USD, EUR, GBP, AED, PHP supported)
- **Crypto Support**: No USDT/USDC
- **Update Frequency**: Daily
- **Format**: JSON
- **CORS**: Supported
- **Example**: `https://v6.exchangerate-api.com/v6/YOUR_API_KEY/latest/USD`

**Pros**:
- Free tier available
- 161 currencies
- Easy to use
- JSON responses
- No credit card required for free plan

**Cons**:
- Requires API key registration
- Does NOT support cryptocurrencies (USDT, USDC)
- Only fiat currencies

#### 2. **CoinGecko API** (https://docs.coingecko.com/)
- **Type**: Cryptocurrency prices and market data
- **Free Tier**: Demo API available (no key required for basic use)
- **Coverage**: 18,000+ coins including USDT, USDC
- **Fiat Support**: Can convert to USD, EUR, GBP, AED, PHP
- **Update Frequency**: Real-time
- **Format**: JSON
- **CORS**: Supported
- **Example**: `https://api.coingecko.com/api/v3/simple/price?ids=tether,usd-coin&vs_currencies=usd,eur,gbp`

**Pros**:
- Free demo API (no key required)
- Supports cryptocurrencies (USDT, USDC)
- Real-time data
- Can convert to multiple fiat currencies
- Very comprehensive

**Cons**:
- Rate limits on free tier
- May require API key for higher usage

### Recommended Solution:

**Use BOTH APIs**:
1. **CoinGecko API** for crypto (USDT, USDC) to fiat conversions
2. **ExchangeRate-API** for fiat-to-fiat conversions (USD, EUR, GBP, AED, PHP)

OR

**Use CoinGecko API ONLY** since it supports both:
- Crypto prices (USDT, USDC)
- Conversion to fiat currencies (USD, EUR, GBP, AED, PHP)
- Fiat-to-fiat can be calculated from crypto base rates

### CoinGecko API Endpoints:

#### Simple Price Endpoint (Free, No Key Required):
```
https://api.coingecko.com/api/v3/simple/price?ids=tether,usd-coin&vs_currencies=usd,eur,gbp,aed,php
```

**Response Example**:
```json
{
  "tether": {
    "usd": 1.00,
    "eur": 0.85,
    "gbp": 0.76,
    "aed": 3.67,
    "php": 59.01
  },
  "usd-coin": {
    "usd": 1.00,
    "eur": 0.85,
    "gbp": 0.76,
    "aed": 3.67,
    "php": 59.01
  }
}
```

### Implementation Plan:
1. Use CoinGecko free API (no key required)
2. Fetch USDT and USDC prices in all fiat currencies
3. Calculate fiat-to-fiat rates from USD base
4. Update every 60 seconds (1 minute) as per user preference
5. Add error handling for API failures
6. Keep simulated data as fallback
