# Space Defense Command - MVP Product Requirements Document

## 1. Project Overview

**What does it do?** A browser-based space tower defense game where I can practice web development while building on my previous Pygame space game experience. Players place turrets to defend against enemy waves.

**Who is it for?** Fellow students and gamers who want a quick strategy game that works instantly in any browser. Also serves as a portfolio piece to show my progression from Python desktop games to web development.
[PRD (1).md](https://github.com/user-attachments/files/24065271/PRD.1.md)# Product Requirements Document (PRD)
# Space Defense Command - Tower Defense Game

## Project Overview
**Project Name**: Space Defense Command  
**Assignment**: H.5.1 "A Quick Prototype" - CSC-113  
**Developer**: Allen  
**Date**: December 2025  
**Development Method**: AI-Assisted Rapid Prototyping

## Background & Context
As a student with experience in Python and Pygame, I'm transitioning to web-based game development for this assignment. This project demonstrates AI-assisted rapid prototyping by building a tower defense game using HTML5 Canvas and JavaScript.

## Problem Statement
Create a functional, engaging tower defense game prototype that:
- Runs entirely in a web browser (single HTML file)
- Demonstrates core tower defense mechanics
- Shows iterative improvement through AI collaboration
- Meets assignment requirements for rapid prototyping

## Target Audience
- Primary: Assignment graders evaluating prototyping skills
- Secondary: Casual gamers who enjoy tower defense games
- Tertiary: Other students learning AI-assisted development

## Core Features (MVP)

### 1. Turret Placement System ✅
**Description**: Players click to place defensive turrets on the map  
**Requirements**:
- 4 turret types: Basic, Rapid, Cannon, Slow
- Click-to-place mechanic with cost system
- Visual feedback for placement validity
- Turret selection UI panel

### 2. Enemy Wave System ✅
**Description**: Enemies spawn in waves with increasing difficulty  
**Requirements**:
- 4 enemy types: Normal, Scout (fast), Tank (tough), Boss
- Wave scaling: 4 enemies + 5 per wave
- Boss enemies every 5 waves
- 10-second break between waves

### 3. Combat & Targeting ✅
**Description**: Turrets automatically target and fire at enemies  
**Requirements**:
- Homing projectiles that track targets
- Splash damage for Cannon turret
- Slow effect for Slow turret
- Visual feedback (explosions, trails)

### 4. Resource Management ✅
**Description**: Players earn and spend resources strategically  
**Requirements**:
- Starting resources: 100
- Earn resources from kills
- Spend on turrets, upgrades, abilities
- Sell turrets for 50% refund

### 5. Upgrade System ✅
**Description**: Turrets can be upgraded to 3 levels  
**Requirements**:
- Click turret to see upgrade options
- Each level improves stats
- Visual indicator of turret level

### 6. Special Abilities ✅
**Description**: Emergency abilities for tough situations  
**Requirements**:
- Nuke (200💎): Damage all enemies
- Freeze (100💎): Stop all enemies for 3 seconds
- Visual effects for each ability

### 7. Game Speed Control ✅
**Description**: Fast forward for slower moments  
**Requirements**:
- Toggle between 1x and 2x speed
- Affects all game elements

## Technical Specifications

### Platform Requirements
- **Target**: Modern web browsers (Chrome, Firefox, Edge, Safari)
- **Format**: Single HTML file with embedded CSS/JS
- **Resolution**: 1000x700 canvas
- **Input**: Mouse click for all interactions

### Technology Stack
- HTML5 Canvas for rendering
- Vanilla JavaScript (no frameworks)
- CSS3 for UI styling
- No external dependencies

## User Experience Flow
1. **Start Screen**: Title, instructions, start button
2. **Gameplay**: Place turrets, defend base, survive waves
3. **Wave Break**: 10-second intermission for strategy
4. **Game Over**: Final score, waves survived, restart option

## Success Metrics
- ✅ Game loads without errors
- ✅ All 4 turret types function correctly
- ✅ All 4 enemy types spawn appropriately
- ✅ Upgrade system works
- ✅ Special abilities function
- ✅ Fast forward works
- ✅ Boss waves trigger every 5 waves
- ✅ Game provides clear feedback

## Out of Scope (Future Versions)
- Sound effects and music
- Mobile touch controls
- Save/load game state
- Multiple maps/levels
- Online leaderboards
- Achievement system

## Development Timeline
| Phase | Duration | Status |
|-------|----------|--------|
| Initial PRD | 30 min | ✅ Complete |
| AI Prototype v1 | 1 hour | ✅ Complete |
| Testing & Comparison | 30 min | ✅ Complete |
| Iteration & Polish | 2 hours | ✅ Complete |
| Documentation | 1 hour | ✅ Complete |

## AI Tools Used
- **Claude (Anthropic)**: Primary development, iteration, documentation
- **ChatGPT (OpenAI)**: Comparison prototype for testing analysis

## Appendix: Turret Stats

| Type | Cost | Damage | Fire Rate | Special |
|------|------|--------|-----------|---------|
| Basic | 50💎 | 25 | 800ms | Balanced |
| Rapid | 75💎 | 10 | 250ms | Fast shots |
| Cannon | 100💎 | 60 | 1500ms | Splash damage |
| Slow | 60💎 | 5 | 600ms | Slows enemies |

## Appendix: Enemy Stats

| Type | Speed | Health | Value | Appears |
|------|-------|--------|-------|---------|
| Normal | 1x | 1x | 1x | Wave 1+ |
| Scout | 2x | 0.4x | 0.8x | Wave 2+ |
| Tank | 0.5x | 2.5x | 2x | Wave 3+ |
| Boss | 0.3x | 10x | 10x | Every 5 waves |


**What problem does it solve?** I want to translate my Pygame game development skills to web technologies for my final project. This creates a playable game that demonstrates both programming ability and game design thinking, while being accessible without Python installation.

## 2. Core Features (MVP - Pick 3)

### Feature 1: Interactive Turret Placement System
- **Description**: Click-to-place turrets around the enemy path - similar to my previous tower defense concepts but web-based
- **Why this matters**: This is the core mechanic that makes tower defense strategic. I want to nail the placement feedback since that's what makes the genre fun
- **Success criteria**: Smooth click-to-place with visual feedback, can't place on path or too close to other turrets

### Feature 2: Improved Bullet Tracking System  
- **Description**: Building on my Pygame homing missile work - turrets fire projectiles that smoothly track moving enemies
- **Why this matters**: This was the main challenge in my previous space games. Getting smooth bullet tracking right will show my programming growth
- **Success criteria**: Bullets curve realistically toward targets, hit moving enemies consistently, visual trail effects

### Feature 3: Wave-Based Progression
- **Description**: Enemies spawn in timed waves with increasing difficulty - different enemy types with varying speed/health
- **Why this matters**: Creates replayability and shows I understand game balance progression from my previous projects  
- **Success criteria**: Each wave feels appropriately challenging, clear indication of wave progress, different enemy behaviors

## 3. User Experience

**What does the user see first?**
- Clean title screen with "Space Defense Command" (keeping it professional for portfolio)
- Simple "Start Game" button - no complex menus needed for MVP
- Brief instructions overlay so players can jump in immediately

**What can they do?**
- Click empty spots to place turrets (visual feedback when affordable/too close/invalid spot)  
- Watch their defense automatically engage enemies (satisfying to see your strategy work)
- Monitor resources and base health through clean UI
- Experience escalating challenge through wave progression

**What happens when they interact?**
- Turret placement: Immediate visual confirmation, range preview, resource cost deduction
- Combat: Smooth projectile animations with impact effects (building on my particle system experience)
- Wave completion: Score updates, resource bonuses, brief pause before next wave
- Game over: Clear final stats, easy restart option

## 4. Technical Constraints

- **Single page application**: One HTML file with embedded CSS and JavaScript
- **Browser compatibility**: Works in Chrome, Firefox, Safari, Edge
- **No external dependencies**: Self-contained code, no libraries needed
- **Responsive design**: Playable on desktop (mobile support nice-to-have)
- **Performance target**: Smooth 60fps with 20+ enemies and projectiles

## 5. Out of Scope (What I'm NOT building yet)

### Future v2 Features (Post-Assignment):
- **Multiple turret types**: Different weapons with unique abilities (missile, laser, rapid-fire from my Pygame version)
- **Upgrade system**: Level up turrets mid-game like my previous upgrade menu implementation  
- **Power-ups and special abilities**: Screen-clearing bombs, temporary boosts
- **Sound effects**: Audio feedback system (would need to learn Web Audio API)
- **Advanced graphics**: Sprite animations, better particle effects
- **Local high scores**: Browser storage for persistent progression
- **Mobile optimization**: Touch controls and responsive layout

### Learning Goals for Later:
- **Backend integration**: Online leaderboards (would need to learn server-side development)
- **Multiplayer features**: Real-time cooperative defense
- **Advanced AI**: Smarter enemy pathfinding and behavior trees  
- **Performance optimization**: Object pooling, spatial partitioning for larger battles

### Assignment Constraints:
- **No external libraries**: Keeping it vanilla JS for now, but might explore frameworks later
- **Single file requirement**: Would normally split into modules for better organization
- **Time limitations**: Focus on core mechanics over polish for this sprint

## 6. Success Metrics

### Assignment Requirements:
- **Functionality**: All core features work reliably in browser testing
- **GitHub workflow**: Proper issues, branches, and PR process demonstrated  
- **AI collaboration**: Successfully iterate with AI tools to improve code quality
- **Portfolio readiness**: Something I'd confidently show to potential employers
- **Documentation**: Clear README and iteration logs showing my learning process

### Gameplay Goals:
- **Intuitive design**: New players can start playing without reading instructions
- **Engaging progression**: Players want to try "just one more wave"  
- **Strategic depth**: Placement decisions meaningfully affect outcomes
- **Performance**: Smooth gameplay with 20+ enemies and projectiles on screen

### Personal Learning Objectives:
- **Web development skills**: Translate my Python/Pygame experience to web technologies
- **Professional workflow**: Experience with PRD → prototype → iterate → deploy cycle
- **AI-assisted development**: Learn to effectively collaborate with AI coding tools
- **Code quality**: Write clean, commented JavaScript that others can understand

### Technical Benchmarks:
- **Load time**: Game starts in <3 seconds on campus internet
- **Cross-browser**: Works in Chrome, Firefox, Safari (assignment requirement)
- **Mobile-friendly**: Playable on phone browsers (stretch goal)
- **No crashes**: 15+ minute play sessions without game-breaking bugs

---

*This PRD reflects my transition from desktop game development to web technologies, while applying professional development practices learned in my Information Technology Studies program.*
