# Brand system

The dashboard is the product — the visual language below is lifted from its CSS (`linkclipper/dashboard/dashboard.css`) so UI and brand stay in lockstep.

## Color

| Role | Hex | Notes |
|---|---|---|
| Base (page) | `#080b18` | Near-black indigo; all surfaces sit on it |
| Surface (glass) | `rgba(26,31,62,.9) → rgba(15,19,40,.84)` | `linear-gradient(170deg)`; no `backdrop-filter` (Brave GPU artifacts) |
| Brand primary | `#7b6cff` (`--brand1`) | Buttons, active states, logo mark |
| Brand secondary | `#b46bff` (`--brand2`) | Gradient partner: `linear-gradient(135deg, --brand1, --brand2)` |
| Brand ink | `#cabcff` (`--brand-ink`) | Logo text, emphasis on dark |
| Text | `#eef0ff` (`--ink`) | Primary copy |
| Text dim | `#9aa3c7` (`--sub`) | Secondary copy, metadata |
| Success | `#34d399` | Preview/play (hover solid `#10b981`) |
| Info | `#7cb0ff` | Open-in-tab (hover solid `#3b82f6`) |
| Danger | `#fb7185` | Delete (hover solid `#ef4444`) |

Aurora background = 4 fixed radial gradients (blue top-left, purple top-right, pink bottom-right, sky bottom-left) on the base. Never animate them; subtlety is the luxury, movement is the risk.

## UI language

- **Glass, no blur.** Translucent gradients + 1px light borders + soft glow read as glass; `backdrop-filter` is banned (see Knowledgebase, Windows GPU artifacts).
- **Purple = action.** Gradients only on primary buttons (Save, New board, Play). Action icon chips hover to *solid* saturated color with dark ink.
- **Type**: system stack, medium weights; titles 500–600, metadata 400. No custom webfonts in the extension (no remote code policy).
- **Logos/wordmark**: "LinkClipper" one word, capital L and C always. The mark is two linked loops on the brand gradient — a saved link, not the former WebCollector `W`. `icons/mark.svg` is the vector reference; keep extension, site and store artwork identical. Do not use text glyphs or emoji as a substitute.

## Store copy voice

Short, concrete, no exclamation marks. Feature-verb-noun ("Save the web you love. Find it again, in one place."). Never describe planned features as existing.
