# 🎲 Liars Dice

A peer-to-peer multiplayer dice game built as a static web application. Play the classic bluffing game with friends without needing a server!

Call via your preferred media, I suggest Discord.

## 🎮 What is Liars Dice?

Liars Dice is a dice game involving bluffing and deduction. Players roll dice in secret and make claims about the total dice on the table. The goal is to catch other players in lies or successfully bluff your way through rounds.

## ✨ Features

- **Peer-to-Peer Connection**: No server required - connect directly to friends using room IDs
- **Real-time Gameplay**: Synchronized dice rolling and revealing across all players
- **Custom Avatars**: Choose from cute animal presets or use your own image URL
- **Animated Dice**: Beautiful rolling animations and visual feedback
- **Responsive Design**: Works on desktop and mobile devices
- **Room Management**: Create private rooms or join existing ones with room codes

## 🚀 Getting Started

### Playing the Game

1. **Open the Game**: Simply open [index.html](index.html) in your web browser
2. **Create or Join Room**:
   - Click "Create Room" to host a new game
   - Or enter a Room ID and click "Join Room" to join an existing game
3. **Set Your Identity**:
   - Enter your name (or use the randomly generated one)
   - Choose an avatar from the presets or enter a custom URL
   - Click "Join" to enter the game
4. **Share Room ID**: Copy the room ID and share it with friends so they can join

### Game Controls

- **🎲 Roll Dice**: Roll new dice for all players
- **👁️ Reveal Dice**: Show everyone's dice values
- **➕ Add Dice**: Add a die to your collection
- **➖ Remove Dice**: Remove a die from your collection

## 🛠️ Technical Details

### Technologies Used

- **HTML5/CSS3**: Modern web standards with responsive design
- **JavaScript (ES6+)**: Game logic and real-time communication
- **PeerJS**: WebRTC peer-to-peer networking library
- **CSS Animations**: Smooth dice rolling and UI transitions

### File Structure

```
├── index.html          # Main game file (complete standalone app)
├── readme.md          # This file
└── avatars/           # Avatar image assets
    ├── bunny.png
    ├── cub.png
    ├── duckling.png
    ├── fox.png
    ├── frog.png
    ├── hedgehog.png
    ├── mouse.png
    ├── penguin.png
    ├── puppy.png
    └── squirrel.png
```

### How P2P Works

The game uses WebRTC through PeerJS to establish direct connections between players:

1. **Host Creates Room**: One player creates a room and gets a unique Room ID
2. **Players Join**: Other players use the Room ID to connect directly to the host
3. **Data Synchronization**: Game state is managed by the host and synchronized to all players
4. **No Server Required**: All communication happens directly between browsers

## 🎯 Game Features

### Dice Mechanics
- Each player starts with 5 dice
- Dice show traditional dot patterns (1-6)
- Visual highlighting when hovering over dice values
- Smooth rolling animations with staggered timing

### Visual Elements
- **Player Cards**: Show name, avatar, and dice for each player
- **Responsive Layout**: Adapts to different screen sizes
- **Visual Feedback**: Hover effects and animations throughout
- **Dark Theme**: Modern dark theme with gradient backgrounds

### Avatar System
- **10 Preset Avatars**: Cute animal illustrations included
- **Custom URLs**: Support for any web-accessible image
- **Persistent Loading**: Images are preloaded to prevent lag

## 🌐 Browser Compatibility

Works in all modern browsers that support:
- WebRTC
- ES6 JavaScript
- CSS Grid/Flexbox
- Async/Await

Tested on Chrome, Firefox, Safari, and Edge.

## 🤝 Contributing

This is a single-file application for simplicity. To contribute:

1. Fork the repository
2. Make your changes to [index.html](index.html)
3. Test the P2P functionality with multiple browser windows
4. Submit a pull request

## 📝 License

This project is open source and available under the MIT License.

## 🎲 How to Play Liars Dice

1. **Setup**: Each player rolls their dice secretly
2. **Bidding**: Players take turns making bids about the total number of dice showing a particular value across all players
3. **Challenging**: Players can challenge the previous bid if they think it's impossible
4. **Resolution**: Reveal all dice to see if the bid was accurate
5. **Elimination**: Losing players lose dice until only one remains

*Note: This implementation provides the dice mechanics - house rules for bidding and challenging should be agreed upon by players!*