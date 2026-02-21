# Fling Punch - Deployment Plan

## Phase 1: Local Testing ✅

1. Open `index.html` in browser
2. Test all mechanics:
   - [ ] Start screen works
   - [ ] Drag/release to fling
   - [ ] Branch grabbing
   - [ ] Swinging physics
   - [ ] Camera follow
   - [ ] Banana collection
   - [ ] Combo system
   - [ ] Game over screen
   - [ ] Restart works
   - [ ] Mobile touch controls

## Phase 2: GitHub Deployment

```bash
cd C:\Users\akvm\.openclaw\workspace\projects\fling-punch
git init
git add .
git commit -m "🐵 Fling Punch - Initial release"
git branch -M main
git remote add origin https://github.com/RazorSharp18/fling-punch.git
git push -u origin main
```

Then enable GitHub Pages:
1. Go to repo Settings
2. Pages section
3. Source: Deploy from branch
4. Branch: main, root folder
5. Save

**Live URL:** https://razorsharp18.github.io/fling-punch/

## Phase 3: play.fun Submission

### Requirements Check
- [x] Single HTML file
- [x] No external dependencies (Three.js via CDN)
- [x] Mobile-friendly
- [x] Works in iframe
- [x] No localStorage requirements (optional enhancement)

### Submission Steps
1. Go to https://play.fun
2. Click "Add Game" (need to login first)
3. Upload `index.html`
4. Fill in details:

**Game Name:** Fling Punch

**Description:**
```
Swing and fling the cutest macaque through an endless jungle! 🐵

Help Punch swing from branch to branch as he climbs higher and higher. Drag to aim, release to fling. Grab bananas for bonus points. Build combos for massive scores.

Simple to learn. Hard to master. Impossible to stop playing.

🍌 How high can you go?
```

**Tags:** arcade, physics, endless, mobile, cute

5. Launch Playcoin (creates game token)
6. Share on X for initial players

## Phase 4: Post-Launch

### Monitor
- Player count
- Feedback in Discord
- Common failure points

### Quick Fixes (if needed)
- Adjust grab radius (too hard/easy)
- Tune launch power
- Fix mobile issues

### Feature Roadmap
1. **Week 1:** Bug fixes based on feedback
2. **Week 2:** Add power-ups (double jump, magnet)
3. **Week 3:** Leaderboard integration
4. **Week 4:** Cosmetic skins

## Marketing

### X Thread
```
🐵 Just launched Fling Punch on @playfun!

Swing your way through an endless jungle with the cutest macaque in gaming.

- Physics-based swinging
- Combo system
- Procedural generation
- Mobile-friendly

Play now: [link]

Built in one night with AI. Let's see how high you can go! 🍌
```

### Discord
Post in play.fun Discord with gameplay GIF

---

**Target Launch:** Today! 🚀
