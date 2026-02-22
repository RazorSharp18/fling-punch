# 🚀 Deploy Fling Punch to Play Fun

## Step 1: Push to GitHub

```bash
cd C:\Users\akvm\.openclaw\workspace\projects\fling-punch
gh repo create fling-punch --public --source=. --push
```

Or manually:
1. Create repo at https://github.com/new (name: `fling-punch`)
2. Push:
```bash
git remote add origin https://github.com/RazorSharp18/fling-punch.git
git push -u origin master
```

## Step 2: Enable GitHub Pages

1. Go to repo → Settings → Pages
2. Source: Deploy from branch
3. Branch: `master`, folder: `/ (root)`
4. Save

**Your game will be live at:** `https://razorsharp18.github.io/fling-punch/`

## Step 3: Submit to Play Fun

1. Go to https://play.fun
2. Click **"Add Game"** (need to login)
3. Fill in:
   - **Name:** Fling Punch
   - **Game URL:** `https://razorsharp18.github.io/fling-punch/`
   - **Description:**
     ```
     Swing and fling the cutest macaque through an endless jungle! 🐵
     
     Help Punch swing from branch to branch as he climbs higher and higher.
     Drag to aim, release to fling. Grab bananas for bonus points.
     Build combos for massive scores!
     
     🍌 How high can you go?
     ```

4. After submission, you'll get a **Game ID**
5. Replace `YOUR_API_KEY` in index.html with your actual API key
6. Replace `gameId: 'fling-punch'` with your actual game ID
7. Push the update

## Step 4: Launch Playcoin

Once approved, click "Launch Playcoin" on your game page to create the token!

---

## SDK Integration Summary

Already integrated per Play Fun docs:

```javascript
// Initialize
const ogp = new OpenGameSDK({ ui: { usePointsWidget: true } });
ogp.init({ gameId: 'YOUR_GAME_ID' });

// Add points during gameplay
ogp.addPoints(heightGain);  // For climbing
ogp.addPoints(50);          // For bananas
ogp.addPoints(comboPoints); // For combos

// End game (auto-login + save)
await ogp.endGame();
```

## Quick Test

Open `index.html` locally to test the game first!
