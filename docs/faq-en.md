---
title: "FAQ: How to pay for ChatGPT Plus, Claude Pro, Cursor and Gemini with a virtual card (Oct 2026)"
description: Why AI subscription payments get declined, how to pay for ChatGPT Plus, Claude Pro, Cursor, Gemini and Midjourney with a prepaid virtual card, what it costs, and what to do after "Your card was declined".
lang: en
---

# FAQ: paying for AI subscriptions with a virtual card

> Updated October 2026. Prices and merchant rules change often; always check the official pricing pages. [Back to index](index.md)

## Why does my card get declined when I subscribe to ChatGPT Plus or Claude Pro?

ChatGPT, Claude, Cursor and Midjourney take card payments on the web mostly through Stripe; Gemini uses Google Payments. Each charge is checked against:

- **Issuing country** of the card (detected from the BIN). If the issuing bank's country is outside the service's supported regions, the card is declined no matter how much money is on it. This is the most common cause.
- **Card type** (debit / credit / prepaid). Some merchants block certain prepaid BIN ranges.
- **Billing address (AVS)**: street, city, state, ZIP and country must match what the issuer has on file.
- **Network exit region**: a region that differs from the billing country adds risk score.
- **3DS authentication** and **balance**, including tax and a pre-authorization hold.

## What are my options?

| Method | Works for | Extra cost | Main trade-off |
|---|---|---|---|
| A bank card issued in a supported country, in your own name | Everything | Usually none | Requires an overseas account |
| Foreign-region Apple ID + App Store gift cards | iOS in-app only (ChatGPT, Claude, some Gemini plans) | Gift-card markup | Not usable for Cursor / Midjourney or web billing |
| Cards issued by trading platforms | Most Stripe merchants | ~1%, usually no monthly fee | Extra account, ID verification, funds must be converted to USD first |
| Prepaid cards funded with local payment methods | Most Stripe merchants | A few dollars to $20 to open, ~3% top-up, some charge annual fees | Several providers shut down in 2024–2025; check track record |
| Single-use virtual cards | One-off payments | Per card | Subscriptions break on renewal |
| Resellers / shared accounts | Mostly ChatGPT | Monthly markup | You hand over your password; usually against terms of service |

## How do I subscribe with a prepaid virtual card?

1. Buy a reloadable card whose issuing country is supported by the service.
2. Subscribe **on the website**, not inside the mobile app (in-app purchases go through Apple / Google and ignore your card).
3. Copy the billing address from the issuer field by field; keep the network exit region in the same country.
4. Keep at least **$25** on the card for a $20/month plan (tax + pre-authorization).
5. Top up before the renewal date.

Official pricing pages: [ChatGPT](https://chatgpt.com/) · [Claude](https://claude.com/pricing) · [Cursor](https://cursor.com/pricing) · [Gemini](https://gemini.google/subscriptions/) · [Midjourney](https://www.midjourney.com/).

## What should I do after "Your card was declined"?

**Do not retry repeatedly.** Several failures in a short time get remembered by risk systems, and many prepaid cards charge a fee even for failed attempts. Instead:

1. Remove the failed card from the service's billing settings.
2. Check issuing country, billing address, balance and network exit region.
3. Wait a few hours, then add the card again.
4. If it still fails, switch method rather than retrying the same kind of card.

"Your card does not support this type of purchase" means the BIN range is blocked — retrying will not help. "Your payment could not be processed" usually means a temporary risk block — stop for several hours.

## Is Claude Pro different?

Claude reviews payments and accounts more strictly than the others. Before paying, check that your region is on the [official supported-countries list](https://www.anthropic.com/supported-countries), keep billing address and login region consistent, and avoid retrying with many different cards. There were reports in 2026 of some Claude accounts in certain regions being suspended; Anthropic did not publish specific reasons. Follow Claude's official terms rather than second-hand rumors.

## What does Pink Card cost? (disclosure: our team builds it)

[Pink Card](https://pinkcard.cc) is a prepaid USD Mastercard / Visa virtual card. Web preset face values start at $110 (custom amount: minimum $100). All fees:

| Item | Fee |
|---|---|
| Issuance | $10 |
| Service fee | 3% of (face value + $10) |
| Top-up | $5 + 5% of (top-up amount + $5); card number stays the same |
| Paying by Alipay | +3% |
| Monthly fee | $2.50 |
| Per transaction | $1, **including failed charges** (failed ones capped at 3 per month) |

Example: a $110 card costs $110 + $10 + 3% × $120 = **$123.60**. Paying for a $20/month subscription for a year adds roughly **$61–75** in fees ([full calculation, in Chinese](fees.md)). It is **not** the cheapest option — no-monthly-fee cards at ~1% cost much less. Its case is convenience: no extra platform account, one card for several subscriptions (ChatGPT, Cursor, Gemini, Google Cloud), reloadable without rebinding.

It cannot be used for App Store / Google Play gift cards or in-app purchases.

---

*For information only; not financial advice. Licensed CC BY 4.0.*
