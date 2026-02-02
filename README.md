# Pixel Puncher – Combo Edition  
A Simple Browser-Based Fighting Game Prototype

![Game Screenshot Placeholder](https://via.placeholder.com/800x400/111133/00ffff?text=Pixel+Punch-Out+Combo+Edition)  
*(Replace with actual screenshot if you take one)*

## Description

Pixel Punch-Out is a minimal, retro-style 1v1 button-masher fighter built entirely in HTML5 Canvas + JavaScript.  

You play as a pixel-art street fighter character (dreads, leather jacket, cargo pants) who throws combos by repeatedly pressing the attack key. Each press advances to the next pose in the sequence, creating the illusion of a combo chain with screen shake and impact glow effects.

Features:
- Cyberpunk/neon background with grid lines
- Single-player (no opponent yet)
- Combo progression via image sequence switching
- Visual feedback: screen shake + yellow flash on every hit
- No health bars or win conditions yet — just pure combo practice fun

Perfect for quick prototyping, learning canvas animation, or as a base for a full fighting game.

## Controls

- **A** or **SPACE** → Attack / Advance combo frame  
  (Each press triggers the next animation pose + effects)

## How to Play / Run

1. Copy the entire code (from the `<!DOCTYPE html>` to `</html>`) into a new file  
   Save as `pixel-punch-out.html`

2. **Option A – Local**  
   Double-click the `.html` file → opens in your browser (Chrome/Firefox recommended)

3. **Option B – Online editors (recommended for quick testing)**  
   - Paste into **JSFiddle** → https://jsfiddle.net  
     - HTML panel: everything from `<canvas>` to `</div>`  
     - CSS panel: the `<style>` content  
     - JS panel: the `<script>` content  
   - Or **PlayCode.io** → https://playcode.io/new → paste whole file into `index.html`

4. Press **A** or **SPACE** repeatedly to see the combo animation!

## Customization

### Add More Combo Frames
Edit the `comboFrames` array in the JavaScript:

```javascript
const comboFrames = [
    "https://i.imgur.com/VMppcev.png",              // starting pose
    "https://i.imgur.com/YOUR_SECOND_POSE.png",     // e.g. wind-up
    "https://i.imgur.com/YOUR_THIRD_POSE.png",      // mid-punch
    "https://i.imgur.com/YOUR_FOURTH_POSE.png",     // full extension
    "https://i.imgur.com/YOUR_FIFTH_POSE.png"       // recovery / kick
    // Add as many as you want!
];
```

- Upload new frames to Imgur / ibb.co → use direct `.png` links  
- The sequence loops automatically

### Tweak Visuals & Feel

- Character size: change `const scale = 2.2;` (smaller = 1.2–1.8, bigger = 2.5+)
- Shake strength: `shake = 1.4;` → higher = more violent shake
- Glow intensity: `glow = 0.9;` → higher = brighter flash
- Animation timing: currently instant on keypress — add delay/cooldown if desired

## Future Ideas / To-Do

- Add health bars (player vs AI opponent)
- Opponent with simple AI (random attacks/blocks)
- Combo scoring / timing bonuses
- Sound effects (punch whoosh, impact hit)
- Win/lose states + restart screen
- Multiple attacks (punch, kick, special)
- Mobile touch support

## Credits / License

Created with help from Grok (xAI) in early 2026.  
Free to use/modify/share for any non-commercial purpose.  
No formal license — just have fun!
 
Enjoy punching pixels! 🥊✨

If you add features or take screenshots, feel free to share — I'd love to see how it evolves!
