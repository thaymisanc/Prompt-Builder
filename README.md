# Fubo Prompt Builder

**Internal tool — Fubo employees only. Do not share externally.**

A browser-based tool that generates production-ready image prompts for [Google Flow](https://labs.google/fx/tools/flow) or any other AI Image Generator. Built to accelerate hero image A/B testing by removing the guesswork from prompt engineering — anyone on the team can generate a high-quality, on-standard prompt in under 5 minutes without prior experience with AI image generation.

---

## Background

The hero section of fubo.tv is one of our highest-leverage conversion surfaces. Historically, producing new hero image variants required photography coordination and design time that could span days. This tool compresses that to minutes by enabling the team to generate AI hero images directly through Google Flow, using prompts that are pre-engineered to meet our visual standards.

---

## How it works

Access here: https://thaymisanc.github.io/Prompt-Builder/
Configure your image using the controls, copy the generated prompt at the bottom, and paste it directly into Google Flow or any other AI Image Generator.

---

## Image types

The tool supports three distinct image types, each with its own set of controls.

### 🏃 Athlete

A player in action inside a real sports environment. This is the primary image type for hero testing.

**Configure:**
- **Sport** — American Football, Soccer, Baseball, MMA, Basketball, Tennis, Hockey, or custom
- **Player action** — sport-specific presets (throwing, sprinting, heading, dunking, etc.)
- **Camera angle** — 3/4 face, front-facing, low angle, side profile, rear, close-up, aerial
- **Body crop** — full body, hip up, waist up, shoulders up, face and chest only
- **Gender** — male or female
- **Skin tone** — light through dark, 5 options
- **Age range** — early 20s through late 30s–40s
- **Build** — muscular & lean, powerfully built, tall & slender, compact & explosive
- **Face visibility** — face visible or hidden (back to camera, helmet low, head down)
- **Expression** — serious, focused, triumphant, aggressive, exhausted, calm, raw emotion
- **Setting** — sport-specific real venue options (live stadiums with fans, never studio shots)
- **Lighting** — match environment, orange, blue, gold rim, green, white, warm golden
- **Kit** — jersey color, number, helmet, league badge, optional fubo logo
- **Lens** — 35mm, 50mm, 24mm ultra-wide, 85mm portrait
- **Tone** — highly saturated, cinematic, desaturated, natural
- **Quality** — 10.7K Ultra-HD, 8K, 4K

### 🏟️ Scene / Setting

A sports venue or stadium with no athlete. The environment itself is the hero — used when the goal is to evoke atmosphere rather than feature a player.

**Configure:**
- Venue type (baseball stadium, soccer stadium, basketball arena, hockey rink, etc.)
- Camera perspective (aerial drone, ground level, upper deck, tunnel entrance, etc.)
- Time of day / atmosphere (golden hour, night floodlights, daytime, dusk, overcast, fog, game day)
- Mood / tone (natural, warm, cool, high contrast, bright, desaturated)
- Lens and quality

### ⭐ Event

A major sporting or cultural moment — championship games, award shows, seasonal events. Prompts are automatically genericized so no team colors, flags, or identifiable branding appear in the output.

**Configure:**
- Category — Championship / Playoff / Finals, Soccer Tournament, Awards & Ceremonies, Cultural & Seasonal, Live Broadcast Moment
- Specific event — pulled from the Fubo 2026 event calendar (World Cup, Super Bowl, NBA Finals, Oscars, etc.)
- Atmosphere — celebration, anticipation, aftermath, broadcast energy, crowd energy, quiet reflection
- Setting — stadium ceremony, on the field, broadcast desk, red carpet, city streets, fan zone
- Tone, lens, and quality

---

## Image quality standards

Every image generated with this tool should be evaluated against these standards before use. The prompts are engineered to hit these targets, but Google Flow output should still be reviewed.

**✅ Aim for:**
- Authentic action captured mid-motion — looks like a real editorial photograph
- Real stadiums with fans visible and blurred in the background
- Natural venue lighting with genuine depth of field
- Realistic skin texture, fabric wrinkles, and sweat detail
- Single clear focus point
- Correct anatomy — exactly 5 fingers per hand
- Consistent, credible uniforms with no conflicting team elements or brand logos
- Diverse representation across athletes and crowds

**❌ Regenerate if you see:**
- CGI, 3D rendering, or an over-edited look
- Studio lighting or fake/floating backgrounds
- Face close-ups — hero images should focus on action and body
- Multiple balls or distracting secondary focal points
- Empty fields or stadiums with no crowd atmosphere
- Copyright logos or registered trademarks on any kit
- Cultural stereotypes or clichés
- Unusual or anatomically incorrect poses
- Impossible stadium geometry

---

## Workflow

1. Configure your image in the Prompt Builder
2. Copy the generated prompt
3. Paste into [Google Flow](https://labs.google/fx/tools/flow) or any other AI Image Generator and generate
4. Review output against the quality standards above — regenerate if needed
5. Bring the approved image into the Hero Composer to add logos, overlay, and export at the correct breakpoint dimensions

---

## Guardrails

The following are enforced by default in every prompt the tool generates:

- **Team-agnostic** — no real team names, colors, or identifiable uniforms
- **No real athlete likenesses** — players are clearly fictional
- **No registered trademarks** — no visible brand logos on kit
- **No cultural stereotypes** — diverse, neutral representation
- **Event prompts are genericized** — "the FIFA World Cup Final" becomes "a major international soccer championship final" in the actual prompt, preventing the AI from inferring team colors or flags

---

## Tips

- **Setting matters most** — choosing a live-game venue with fans consistently produces more authentic-looking output than any other single setting
- **Face visibility off** — hiding the face (back to camera, helmet low) often produces more usable hero images since AI struggles with realistic faces at scale
- **Less saturated = more real** — "Natural / Realistic" tone tends to produce less AI-looking output than "Highly Saturated"
- **35mm lens** — closest to editorial sports photography and usually the most natural-looking result
- **If output looks too perfect** — it's probably too photorealistic/plastic. Adjust tone to desaturated and regenerate
- **If logos or team marks appear on the kit** — the prompt guardrail failed. Regenerate and note the prompt settings that caused it

---

## Questions or feedback

Reach out to Thaymisan Cavalcante on Slack or open an issue in this repo.
