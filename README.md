# Hair ID — Interactive Prototype

An interactive prototype for **IAT 333 — Final Design Solution Pitch**.

Hair ID is one app that carries a client's **precise haircut spec** from chair to chair, and lets both the client and the barber **see the cut before it happens**. It is our converged solution to a communication problem we studied: haircut consultations break down because clients lack the vocabulary to describe what they want, and barbers lack a shared, precise medium to confirm it.

## Live demo

👉 **[Open the prototype](https://REPLACE-WITH-YOUR-LINK)**

*(Replace the link above with your GitHub Pages or Netlify URL once deployed. To run it locally instead, just open `index.html` in any browser — no setup required.)*

## The problem

From our field observations and interviews:

- **Who** — Clients who lack structural hair vocabulary, and busy barbers working under time pressure.
- **What** — Vague, imprecise consultations ("just a trim", "clean up the sides") that don't map onto a person's real head shape, hair density, or growth patterns — leading to anxiety and mismatched cuts.
- **Evidence** — 81.9% of people feel anxious seeing a new stylist; 1 in 3 report frequent bad cuts.

**How might we** build a reliable, shared visual and conceptual vocabulary during the pre-cut consultation window — so expectations align and outcomes are predictable?

## Our converged solution

This prototype merges two of our concepts into a single product:

| From | Contributes |
|------|-------------|
| **Concept 1 — Hair Profile Record** | Multi-angle spec, dye history, and a shareable QR code that travels between barbers |
| **Augmented Photo Preview** | A visual try-on that maps a chosen style onto the client's own head, plus a barber confidence check |

The flow: **Build profile → Preview a new style → Lock & share QR → Barber reads the spec & rates confidence → 360° update after the cut.**

## What you can do in the prototype

**Client side (Ravi)**
- View a saved haircut profile: spec sheet, four saved views (front / left / right / back), and barber notes
- Try a new style — switch between **Men's** and **Women's** styles
- Adjust the look live on a parametric head:
  - Short cuts: top length, fade height, clipper guard
  - Long styles: overall length and layering (soft / medium / choppy)
- Lock the look and generate a shareable **QR code + link**
- See a timeline history, including an auto-flagged **dye record**

**Barber side**
- Scan the client's Hair ID to load the full spec instantly (no account needed)
- See a **dye alert** and the client's locked target preview
- Rate **confidence** (high / medium / low); low confidence surfaces a suggested adjustment to send back to the client
- Record a **360° scan** after the cut to update the profile for any future barber

Use the **Client / Barber** switch in the left panel to move between the two roles.

## Suggested demo path

1. Start as **Client** → **Try a new style** → **Women's → Long layers**
2. Drag **Length** from 34 cm down to 20 and back; switch **Layering** to Choppy
3. **Lock this look & share** → view the QR code
4. Switch to **Barber** → **Simulate scan** → review the spec, dye alert, and target preview
5. Rate confidence **Medium** to see the adjustment suggestion
6. **Cut done → update profile** → record the 360° scan → the client's history updates

## Running locally

No build step, no dependencies. Either:

- Double-click **`index.html`**, or
- Open the folder in VS Code and use the **Live Server** extension.

## Files

| File | Description |
|------|-------------|
| `index.html` | Self-contained prototype (HTML + CSS + JS in one file) — use this to deploy or submit |
| `hair-id-prototype.html` | Same prototype with styles in a separate file |
| `styles.css` | Stylesheet for `hair-id-prototype.html` (must sit in the same folder) |

*Note: `hair-id-prototype.html` needs `styles.css` beside it to display correctly. `index.html` needs nothing else.*

## Built with

Plain HTML, CSS, and vanilla JavaScript. The style previews are drawn as parametric SVG, so the head updates live as the controls change — no image assets required.

## Team

IAT 333 — Project Group. This submission counts for the whole group.
