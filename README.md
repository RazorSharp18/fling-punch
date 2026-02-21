# 🐵 Fling Punch

**Swing Your Way Home!**

A physics-based vertical climber where you help Punch, an adorable baby macaque, swing from branch to branch to reach the sky.

## 🎮 Play Now

[Play on GitHub Pages](https://razorsharp18.github.io/fling-punch/) *(deploy pending)*

## 🎯 How to Play

- **Drag** anywhere on screen to aim
- **Release** to fling Punch
- **Grab branches** automatically on contact
- **Collect bananas** for bonus points
- **Build combos** by grabbing branches quickly

## ✨ Features

- 🎨 Cute 3D macaque character with expressions
- 🌿 Procedurally generated jungle
- 🍌 Collectible bananas
- 🔥 Combo system for skilled play
- 🔊 Procedural sound effects (no audio files needed)
- 📱 Mobile-friendly touch controls
- 🎯 Satisfying physics-based swinging

## 🛠️ Technical

- Built with Three.js (single HTML file)
- No dependencies beyond Three.js CDN
- Mobile-optimized (60fps target)
- Object pooling for performance
- Procedural audio generation

## 🚀 Deployment

### GitHub Pages
```bash
git init
git add .
git commit -m "Initial release"
git remote add origin https://github.com/RazorSharp18/fling-punch.git
git push -u origin main
# Enable GitHub Pages in repo settings
```

### play.fun
1. Go to https://play.fun
2. Click "Add Game"
3. Upload `index.html`
4. Set game details:
   - **Name:** Fling Punch
   - **Description:** Swing and fling the cutest macaque through an endless jungle! Grab branches, collect bananas, and reach for the sky. How high can you go?
5. Launch Playcoin

## 📊 play.fun Integration

The game is ready for play.fun's platform SDK. When the SDK is available:

```javascript
// Already included in code
if (window.PlayFun) {
  PlayFun.ready();
  PlayFun.gameStart();
  PlayFun.gameOver({ score: finalScore, height: maxHeight });
}
```

## 🎨 Credits

- Game Design & Development: Steve (AI) + spitfire1337
- Character inspired by Punch the baby macaque
- Built for play.fun platform

## 📝 License

MIT License - Do whatever you want with it!

---

*Made with 🍌 and ❤️*
