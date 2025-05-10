# Bubble Gun Game Project Report - CMPE496 HW-3

## Contributors

- Yasin Atlı - 2020400246
- Enes Başer - 2020400141

## 1. Application Description

Bubble Gun is an interactive web-based game where players aim to pop bubbles using a virtual gun. The game is designed to provide an engaging and fun experience while incorporating key principles of Human-Computer Interaction (HCI). Players can choose difficulty levels, track their scores, and enjoy sound effects for a more immersive experience. The game also includes accessibility features such as a color-blind friendly mode and multiple input methods.

## 2. Design and Implementation

### Architecture

The game is implemented as a single HTML file containing three main components:

1. HTML Structure
2. CSS Styling
3. JavaScript Game Logic

### Key Implementation Details:

#### HTML Structure:

- Game container for the main play area
- Control panel for game options
- Vertical health and heat bars
- Theme toggle button
- Score display elements

#### CSS Features:

- Responsive layout
- Theme-based styling (dark/light modes)
- Smooth animations for visual feedback
- Vertical progress bars for health and heat
- Dynamic color changes based on status

#### JavaScript Components:

1. **Core Game Loop**:

- RequestAnimationFrame for smooth animation
- Collision detection system
- Object movement and updating
- Game state management

2. **Player Systems**:

- Health management
- Gun heat mechanics
- Movement control
- Shooting mechanics

3. **Bubble Management**:

- Dynamic creation and removal
- Health system
- Shooting AI
- Movement patterns

4. **Game State**:

- Score tracking
- Difficulty management
- Reset functionality
- Theme switching

### Implementation Challenges and Solutions:

1. **Bubble Shooting Mechanics**:

- Challenge: Inconsistent shooting behavior
- Solution: Implemented individual shooting cooldowns and proximity-based shooting probability

2. **Heat Management**:

- Challenge: Balance between playability and challenge
- Solution: 10-shot limit with graduated cooling system

3. **Game Over Logic**:

- Challenge: Multiple end conditions
- Solution: Simplified to health-based game over condition

4. **UI Layout**:

- Challenge: Intuitive display of game status
- Solution: Vertical bars for health and heat outside game frame

## 3. Libraries and Tools Used

The game is built using vanilla web technologies without external dependencies:

### Core Technologies:

1. **HTML5**

   - Canvas-free implementation
   - Semantic markup
   - Modern HTML features

2. **CSS3**

   - Custom properties for theming
   - Flexbox for layout
   - Transitions and animations
   - Media queries for responsiveness

3. **Vanilla JavaScript**
   - ES6+ features
   - RequestAnimationFrame for game loop
   - DOM manipulation
   - Event handling

### Development Approach:

- No external libraries or frameworks
- Pure browser technologies
- Object-oriented design patterns
- Responsive design principles

### Browser Features Used:

- Local storage for best score persistence
- DOM manipulation for game elements
- CSS transitions for smooth animations
- Event handling for user input

## ChatGPT Prompts Used

During the development of the Bubble Gun Game, ChatGPT was used to accelerate feature design, fix bugs, and align the implementation with core HCI principles. Below is a categorized summary of the prompts used throughout the development process:

### A. Initial Game Mechanics and Core Structure

- **“Implement a simple game which is bubble gun…”**  
  Requested basic shooting mechanics where the player controls a gun at the bottom of the screen and bubbles fall from the top. Prompted the development of core loop logic, bubble generation, and object control.

- **“Objects should have health, and bubbles should be populated at the bottom…”**  
  Introduced health-based logic for both the player and bubbles, with game over triggered by bubble stacking or health depletion.

- **“Score should be based on shot bubbles and should depend on difficulty.”**  
  Guided the development of a dynamic scoring system and difficulty-based bubble behavior.

- **“Best score should be shown and reset option should be included.”**  
  Informed the implementation of persistent best score tracking via local storage and a reset button in the UI.

### B. Bug Fixing and Game Logic Corrections

- **“There is a bug — game over logic triggers too early…”**  
  Helped correct early termination issues by refining game over logic based solely on player health reaching zero.

- **“Health bar should be outside the game frame and shown vertically…”**  
  Improved visual clarity and game aesthetics by placing the health indicator outside the active play area.

- **“After some point, bubbles are not shooting anymore…”**  
  Prompted the addition of cooldown timers and randomness to bubble shooting logic to ensure continuous challenge.

### C. UX, Sound, and Visual Feedback

- **“I want to add sound when a bubble is destroyed and a game over sound.”**  
  Enhanced feedback using HTML5 `<audio>` elements, improving immersion and responsiveness of game events.

- **“Please add color-blind friendly mode — a toggle for high contrast bubbles.”**  
  Introduced accessibility features through a dedicated toggle button to switch between standard and color-blind safe visuals.

### D. User Interaction and HCI-Oriented Additions

- **“I want to add a tutorial or ‘How to Play’ popup.”**  
  Helped implement a modal explaining gameplay mechanics, controls, and difficulty levels — supporting the “Help and Documentation” principle.

- **“Add keyboard controls (A/D or arrows for movement, space/enter for shooting).”**  
  Enabled multi-modal input for improved accessibility and player preference.

- **“Show post-game feedback summary with accuracy, time survived, and bubbles destroyed.”**  
  Informed the design of a results screen for self-assessment, reinforcing the “Feedback and Evaluation” principle.

## HCI Principles Applied

### 1. Visibility

- Clear visual feedback for all actions
- Distinct color coding for different game elements
  - Red gun for player identification
  - Colorful bubbles with visible health numbers
  - Yellow bullets for player projectiles
  - Red bullets for enemy projectiles
- Prominent display of game status (health, heat, score)
- Visual indicators for overheating and cooling down

### 2. Feedback

- Immediate visual response to player actions
- Color changes in heat bar indicating weapon status
- Health bar color changes based on player condition
- Score updates instantly upon successful hits
- Bubble health numbers decrease visibly when hit
- Visual feedback when gun is overheated (pulsing animation)
- Theme toggle provides immediate visual confirmation

### 3. Consistency

- Uniform visual style throughout the game
- Consistent control scheme
- Predictable behavior patterns
- Coherent color scheme in both dark and light themes
- Standard button and control layouts

### 4. User Control and Freedom

- Ability to reset game at any time
- Theme switching option
- Difficulty level selection
- Freedom of movement within game boundaries
- Controlled shooting mechanics with heat management

### 5. Error Prevention

- Clear boundaries for player movement
- Visual warnings before overheating
- Obvious visual cues for dangerous situations
- Confined game area preventing off-screen actions

### 6. Recognition Rather Than Recall

- Visual indicators for all game states
- Clear labeling of controls and status bars
- Intuitive color coding
- Visible difficulty settings

### 7. Flexibility and Efficiency

- Simple, intuitive controls (mouse movement and clicking)
- Multiple difficulty levels for different skill levels
- Adaptive challenge (bubbles shoot more when closer)
- Quick reset option for new games

### 8. Aesthetic and Minimalist Design

- Clean, uncluttered interface
- Essential information only
- Clear visual hierarchy
- Minimal color palette with good contrast
- Simplified game mechanics

### 9. Accessibility

- High contrast visuals
- Clear visual feedback
- Simple control scheme
- Dark/light theme options for different lighting conditions
- Readable text and numbers

### 10. Help and Documentation

- Simple, self-explanatory mechanics
- Visual tutorials through design
- Clear labeling of all game elements
- Intuitive learning curve

## Conclusion

The Bubble Gun Game demonstrates the capability of modern web technologies to create engaging interactive experiences without external dependencies. The project successfully implements core gaming concepts while maintaining clean code structure and following best practices in web development.
