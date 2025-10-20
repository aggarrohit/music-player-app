# MusicRewards App

This is a react native expo app created using react native track player for playing music and rewarding users for completing the challenge.

## 🚀 Run Instructions

- git clone https://github.com/aggarrohit/music-player-app.git
- cd music-rewards-app
- npm install
- npx expo prebuild --clean
- npx expo run:ios

## 📁 Project Structure

This structure follows Belong's mobile app architecture patterns:

```
src/
├── app/                    # Expo Router pages
│   ├── (tabs)/
│   │   ├── index.tsx       # Home screen with challenge list
│   │   ├── profile.tsx     # Profile with user progress
│   │   └── _layout.tsx     # Tab navigation setup
│   ├── (modals)/
│   │   ├── player.tsx      # Full-screen audio player
│   │   └── _layout.tsx     # Modal navigation setup
│   └── _layout.tsx         # Root layout
├── components/
│   ├── ui/                 # Glass design system components
│   │   ├── GlassCard.tsx
│   │   ├── GlassButton.tsx
│   │   └── PointsCounter.tsx
│   └── challenge/          # Challenge-specific components
│       ├── ChallengeCard.tsx
│       └── ChallengeList.tsx
├── hooks/                  # Business logic hooks
│   ├── useMusicPlayer.ts
│   ├── usePointsCounter.ts
│   └── useChallenges.ts
├── stores/                 # Zustand stores
│   ├── musicStore.ts
│   └── userStore.ts
├── services/               # External services
│   └── audioService.ts
├── constants/              # Theme and configuration
│   └── theme.ts
└── types/                  # TypeScript definitions
    └── index.ts
```

## 🎵 Audio Files

The assessment uses these pre-hosted tracks:

- **Track 1:** Camo & Krooked - All Night (3:39, 150 points)
- **Track 2:** Roni Size - New Forms (7:44, 300 points)

URLs and sample data are in [`./assets/audio/README.md`](./assets/audio/README.md)
