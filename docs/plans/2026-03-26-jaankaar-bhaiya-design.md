# Jaankaar Bhaiya — "The Accountability Arc" Design

## Overview

Single-page HTML prototype showing Amit's full journey with Jaankaar Bhaiya across 3 acts in one chat flow. Demonstrates the accountability buddy product: goal setup, weekly check-ins with real data, and milestone celebration.

## Frame

- Single phone frame (390x844), centered, dark background
- Header: JBIQ video avatar + "Jaankaar Bhaiya" + "Tera bada bhai"
- Persona dropdown: Amit (primary, fully built), Priya & Raju (secondary, simpler flows)
- Same engine pattern as Apna Dost: typing indicator, TTS via ElevenLabs, chip-based branching, auto-advance with listening state

## Act 1: "Pahli Baat" — First Meeting & Goal Setup

1. Welcome message — casual intro, not corporate
2. Bhaiya asks what Amit's goal is
3. Amit says ₹2 lakh savings
4. **Goal Breakdown Card**: ₹2,00,000 target, ₹16,700/month, current JioPay spending summary with simple colored bars
5. Bhaiya suggests recording a voice commitment
6. **Voice Commitment Card**: fake waveform recording animation → "Saved" state
7. Bhaiya: "Har hafte poochhunga. Bhagna mat."

## Time Skip

Cinematic card: "8 hafte baad..." with mini progress indicator ₹0 → ₹1.1L

## Act 2: "Hisaab Kitaab" — Week 8 Check-in

1. Context card (memory from last session)
2. Bhaiya greeting referencing gym/spending
3. Branching conversation via chips
4. **Spending Card**: colored bars for Swiggy, JioMart, Recharge, Petrol + total
5. Bhaiya reality check on Swiggy (direct, practical tone)
6. Branching responses with practical suggestions
7. **Progress Card**: simple bar or ring showing 55%, ₹1.1L saved, ₹2L target
8. **Nudge Card**: "Next week Swiggy max ₹1,000. Deal?"

## Time Skip

"4 mahine baad..." progress at 75%

## Act 3: "Sun Apni Awaaz" — Month 10 Milestone

1. **Milestone Card**: ₹1,50,000 saved, 75% complete
2. Bhaiya: "Yaad hai kya bola tha? Sun apni awaaz."
3. **Voice Playback Card**: play button + waveform + progress bar (plays a pre-recorded clip)
4. Bhaiya reflection — real, not cringe
5. **Journey timeline**: simple dots showing ₹0 → ₹50K → ₹1L → ₹1.5L → ₹2L
6. Next goal chips
7. Summary sign-off card

## Tone

- Direct: "₹4,200 Swiggy pe gaye. Serious hai?"
- Practical: "Tiffin service le. ₹3,000 mahine mein."
- Teasing (light): "Swiggy wale tujhe naam se jaante honge"
- Warm when it counts: "Tu kar raha hai. Numbers dikha rahe hain."
- No motivational poster quotes. No "You can do it!" energy.
- Hindi/Hinglish — natural, how real people talk

## Technical

- JDS design tokens for all colors/spacing/type
- JioType font from CDN
- JBIQ video avatar (idle/speaking/listening states)
- ElevenLabs TTS with Hindi multilingual model
- Flow engine matching Apna Dost pattern (data-driven, branching)
- GitHub Pages deployment

## Card Types (clean, not over-designed)

1. **Context Card** — warm background, memory text
2. **Goal Breakdown Card** — big number + monthly math + spending bars
3. **Voice Card** — waveform + record/play states
4. **Spending Card** — colored bars with labels and amounts
5. **Progress Card** — bar or ring with percentage + numbers
6. **Nudge Card** — icon + text + action chips inline
7. **Time Skip Card** — centered, cinematic, mini progress
8. **Milestone Card** — celebration with timeline
9. **Summary Card** — mood arc + next meeting time
