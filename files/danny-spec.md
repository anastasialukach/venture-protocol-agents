# Danny — SPEC.md

**Project:** AI Runway Calculator  
**Agent:** Danny (Builder)

---

## Overview

A web-based calculator that compares traditional startup runway with AI-accelerated runway.

---

## UI/UX Specification

### Layout
- Single page application
- Dark theme (#0d0d12 background)
- Card-based design
- Mobile responsive (stack on mobile)

### Color Palette
- Background: #0d0d12
- Card: #16161e
- Border: #2a2a3a
- Text: #f0f0f5
- Text muted: #8888a0
- Accent: #6366f1 (purple)
- Green: #10b981
- Red: #ef4444

### Typography
- Primary: Inter
- Mono: JetBrains Mono (numbers)

---

## Input Fields

| Field | Type | Default | Validation |
|-------|------|---------|------------|
| Cash in Bank | Number | 500,000 | > 0 |
| Monthly Burn | Number | 50,000 | > 0 |
| Team Size | Select | 1 | 1, 3, 8, 15 |
| Scope | Select | MVP | MVP, Product, Scale |

---

## Calculations

### Traditional Runway
```
runway_months = cash / burn_rate
```

### AI-Accelerated Runway
```
ai_orchestrator_cost = $2,000/month
ai_tools_cost = $500/month
team_reduction = max(0, team_size - 1)
reduced_burn = (team_reduction × $8,000) + $2,000 + $500
ai_months = cash / reduced_burn
```

### Speed Multipliers
- MVP: 4x faster
- Product: 3.5x faster
- Scale: 3x faster

---

## Output Display

### Traditional Card
- Border: Red (#ef4444)
- Value: months (large)
- Label: "months at current burn"

### AI Card
- Border: Green (#10b981)
- Value: months (large)
- Label: "months with AI agents"

### Savings Card (when AI enabled)
- Shows dollar savings
- Background: gradient green

---

## Tool Recommendations

| Scope | Tools |
|-------|-------|
| MVP | Make.com, Bubble, ChatGPT, Webflow, Airtable |
| Product | Cursor, Replit, Vercel, LangChain, Zapier |
| Scale | LangChain, AWS, PostgreSQL, OpenAI API, Stripe |

---

## Testing

- [x] iPhone SE
- [x] iPhone 14 Pro
- [x] Desktop Chrome
- [x] Desktop Safari

---

## Deployment

- GitHub Pages: ✅ Live
- URL: https://anastasialukach.github.io/venture-protocol-agents/

---

*SPEC complete*
