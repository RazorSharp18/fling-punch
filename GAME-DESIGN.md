# Fling Punch - Game Design Document

## Overview

**Title:** Fling Punch
**Tagline:** "Swing. Fling. Find Your Way Home."
**Genre:** Physics-based vertical climber with swing mechanics
**Platform:** Web (HTML5), targeting play.fun

## Core Concept

Punch is a baby macaque trying to swing his way home through a procedurally generated jungle. Players drag to aim and release to fling Punch from branch to branch. The higher you go, the more points you earn.

**Why Fling Mechanics?**
- Punk Fling has 106 players (highest on play.fun)
- Simple to learn, hard to master
- Naturally creates "one more try" moments
- Works perfectly with touch/mobile

## Gameplay

### Controls
- **Drag anywhere** - Aim trajectory (shows arc preview)
- **Release** - Launch Punch
- **Auto-grab** - Punch automatically grabs branches he touches

### Mechanics
1. **Swing Physics** - Realistic pendulum motion when hanging
2. **Momentum Transfer** - Timing release for maximum distance
3. **Branch Types:**
   - Standard (brown) - Normal grab
   - Slippery (green/wet) - Can't hold long
   - Bouncy (pink flowers) - Extra launch power
   - Moving (vines) - Swing back and forth

### Scoring
- 1 point per meter climbed
- Combo multiplier for quick successive grabs
- Bonus points for near-miss obstacles
- Golden banana collectibles (50 points each)

## Visual Style (from Art Director)

### Punch Character
- Baby macaque with oversized head (60/40 ratio)
- Large shiny eyes with double highlights
- Pink face with blush marks
- Expressive tail (curls when happy, droops when falling)
- Gray-brown fur with lighter chest

### Environment
- Parallax jungle backgrounds (5 layers)
- Warm peach/green/gold palette (sunrise)
- Floating particles (dust motes, fireflies)
- Fog at lower depths

### Effects
- Jump: Dust puff + squash/stretch
- Grab: Leaf particles + screen shake
- Fall: Speed lines + sad expression
- Score popup: Gold sparkles

## Technical Implementation (from Engineer)

### Architecture
- Single HTML file with embedded Three.js
- Custom swipe/drag controller (no libraries)
- Object pooling for branches/particles
- Fixed timestep game loop (60fps target)

### Mobile Optimization
- Max 2x pixel ratio
- Shared geometries/materials
- <100 draw calls
- No shadows on mobile

## Emotional Hooks (from Designer)

### Story
Punch fell from his tree during a storm. His stuffed monkey friend is waiting at the top. Every session is a new attempt to climb back home.

### Audio
- Soft chirping on grab
- Wind whoosh on big flings
- Gentle music that builds with height
- Sad whimper on fall

## play.fun Integration

### Token Economy
- Points convert to tokens at end of session
- Daily bonus for first play
- Leaderboard rewards (top 10 get bonus)

### Social
- Share best height as image
- Ghost runs (race previous best)
- Weekly challenges

## MVP Features (Week 1)

1. ✅ Core swing/fling physics
2. ✅ Procedural branch generation
3. ✅ Basic Punch character (3D sphere with face)
4. ✅ Score tracking
5. ✅ Mobile touch controls
6. ✅ Particle effects
7. ✅ Sound effects (procedural)
8. ✅ Game over / restart

## Post-MVP

- Cosmetic skins for Punch
- Power-ups (double jump, magnet, etc.)
- Daily challenges
- Leaderboard integration
- Achievement system

---

*Let's build something that makes people smile.*
