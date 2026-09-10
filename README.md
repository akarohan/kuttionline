# 🃏 Kutti Online

> A multiplayer Indian card game built for Android — featuring real-time online rooms, classic Kutti gameplay, player interaction, and a dark maroon & gold interface.

**Kutti Online** is an Android multiplayer card game designed around the traditional Kutti gameplay experience, rebuilt as a fully interactive online game.

Players can create or join rooms, play together remotely, follow the complete Kutti game flow, request cards from other players, become winners, and ultimately determine who is left as the Kutti.

---

## 📱 Release

### Current Release

**Kutti Online — Android**

- Platform: Android
- Orientation: Portrait only
- Multiplayer: Online
- Maximum players: 10
- Minimum players: 2
- Backend: Firebase Realtime Database
- Authentication: Firebase Anonymous Authentication
- Game modes:
  - Original Kutti
  - Blind Kutti

### Installation

Download the latest APK from the **GitHub Releases** section.

> Android may display a warning when installing an APK downloaded outside Google Play. This is expected for privately distributed Android applications.

---

# 🎮 Game Overview

Kutti is a multiplayer card game where players are progressively eliminated through card distribution, rounds of play, risk management, and player-to-player requests.

The objective is not simply to get rid of cards.

Players must manage their cards while trying to avoid becoming the final remaining active player.

The game progresses through two major stages:

1. **Original Kutti Distribution**
2. **Main Game**

The exact flow depends on the selected game mode.

---

# ✨ Features

## 🌐 Online Multiplayer

- Real-time multiplayer rooms
- 2–10 players
- Create a private room
- Join an existing room using a room code
- Player names displayed throughout the game
- Persistent player seating order
- Host-based room management
- Host transfer when the host explicitly leaves
- Player ready system
- Player kick functionality
- Reconnection support
- Multiplayer state synchronization through Firebase

---

## 🏠 Room / Lobby System

Players begin from the main entry screen.

### Create Room

A player can:

- Enter their name
- Select a game mode
- Create an online room
- Become the room host
- Invite other players using the room code

### Join Room

Players can enter a room code to join an existing game lobby.

### Lobby Features

- View all players
- View player names
- View player seats
- Ready / unready status
- Host indicator
- Host controls
- Kick players
- Start game when requirements are satisfied
- Leave room

### Host Management

The host can:

- Start the game
- Remove players from the lobby
- Manage the room before the game begins

If the host explicitly leaves while other players remain, host ownership is transferred to the remaining player with the lowest seat number.

A temporary network disconnect does not automatically transfer host ownership.

---

# 🃏 Game Modes

## Original Kutti

The classic game mode.

The Original Kutti flow includes:

- Initial card distribution
- Central card distribution phase
- Passing cards
- Main Game
- Suit-following gameplay
- Risk Holder mechanics
- Break rounds
- Winner requests
- Multiple winners
- Final Kutti

---

## Blind Kutti

A separate Kutti game mode intended for the blind variant of the game.

The game mode is selectable directly from the Entry Screen and is represented separately in the lobby/game flow.

---

# 🃏 Deck

Kutti uses a standard:

**52-card deck**

There are:

- 4 suits
- 13 ranks per suit
- No Jokers

### Suits

- ♠ Spades
- ♥ Hearts
- ♦ Diamonds
- ♣ Clubs

### Rank Order

Cards are ranked:

```text
A
K
Q
J
10
9
8
7
6
5
4
3
2
