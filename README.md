# Bubble Gun Game Project Report - CMPE496 HW-3

## Contributors

- Yasin Atlı - 2020400246
- Enes Başer - 2020400141

## 1. Application Description

Bubble Gun is an interactive web-based game where players aim to pop bubbles using a virtual gun. The game is designed to provide an engaging and fun experience while incorporating key principles of Human-Computer Interaction (HCI). Players can choose difficulty levels, track their scores, and enjoy sound effects for a more immersive experience. The game also includes accessibility features such as a color-blind friendly mode and multiple input methods.

## 2. Design and Implementation

The game was designed with simplicity and engagement in mind. The following steps were taken during the development process:

- **Game Logic**: Bubbles are generated dynamically and move across the screen. Players aim and shoot at the bubbles to pop them. The game ends when the player's health reaches zero.
- **Health and Scoring**: A health bar is displayed next to the game frame, and the score is updated based on the number of bubbles popped.
- **Sound Effects**: Audio feedback is provided for bubble pops and game-over events.
- **Accessibility**: A toggle button allows players to switch to a high-contrast color scheme for better visibility.
- **Input Methods**: Players can use mouse, touch, or keyboard controls to interact with the game.
- **Post-Game Feedback**: A summary screen displays the player's final score, accuracy, bubbles destroyed, and time survived.

## 3. Libraries/Tools Used

- **HTML5**: For structuring the game interface.
- **CSS3**: For styling the game elements.
- **JavaScript**: For implementing the game logic, including bubble generation, collision detection, and scoring.
- **Audio Files**: For sound effects (`buble_pop.mp3` and `game_over.mp3`).
- **Browser Developer Tools**: For debugging and testing the game.

## 4. ChatGPT Prompts Used

The following prompts were used to generate the single HTML page and JavaScript code for the game:

- "Implement a simple game which is bubble gun and object should have health bubbles should be populated at the bottom so that object's mobility decrease if it miss bubbles. And if populated height of any of the column of bubbles reach top game is over. Best score should be shown and reset game option should be seen. Score should be based on shooted bubble and hardness level should be chosen such that arising of bubbles should be regulated based on hardness level"
- "Object should be placed at the bottom and bubbles should propagate down from top to bottom"
- "Can you please make size of random between two acceptable sizes and also maybe you can change logic for finishing game logic"
- "There is bug gaming over logic it overs earlier i dont understand make overing logic such that health of the object reaches to zero object health should be seen at near like bar. And also falling bubbles should also be shooting please"
- "Gaming logic should be barely on health reaches to zero barely. Please rearrange it also health bar should be out of game frame but next to screen vertically"
- "After some point bubbles are not shooting the object why at initial they are shooting but then not and also they might be more offensive"
- "I would like to add sound when bubble is destroyed and also 'Game Over' sound. This way, it applies the 'Feedback' principle. Audio cues make the interface feel more responsive and immersive. Use the HTML <audio> element and play sounds with new Audio('sound.mp3').play() on events."
- "I also want to implement that Color-Blind Friendly Mode. Add toggle button for alternative high-contrast or pattern-based color scheme for bubbles and bullets. This applies 'Accessibility' and 'User Preference'. Not everyone can distinguish red from green."
- "I would like to add Tutorial or 'How to Play' Popup. A modal or overlay that shows how to move, how to shoot, what bubbles and bullets do, what the difficulty means. This applies 'Help and Documentation'. Users shouldn’t guess how to interact."
- "I also want to add Keyboard Controls. Use left/right arrows or A/D to move, Spacebar or Enter to shoot. This applies 'Multiple Modes of Input' — improves efficiency and accessibility, e.g., for players with motor impairments."
- "I want to add Post-Game Feedback Summary. When game ends, show: Final score, Accuracy (% of shots that hit), Bubbles destroyed, Time survived. This applies 'Feedback and Evaluation' and helps users reflect on their performance."
- "Implement functionality such that a user can disable or activate sound effect with settings popup."

These prompts guided the development of the game and ensured that key features and HCI principles were implemented effectively.

## 5. HCI Principles Applied

1. **Feedback**: Immediate visual and auditory feedback is provided when a bubble is popped, reinforcing player actions.
2. **Simplicity**: The interface is minimalistic, ensuring that players can focus on the gameplay without distractions.
3. **Consistency**: The design and controls remain consistent throughout the game, providing a seamless experience.
4. **Error Prevention**: The game minimizes errors by restricting interactions to the game canvas.
5. **Engagement**: Dynamic elements like moving bubbles, sound effects, and a gradually increasing difficulty curve keep the player engaged.
6. **Learnability**: The game is easy to learn, with intuitive controls and clear objectives.
7. **Accessibility**: A color-blind friendly mode ensures that the game is accessible to a wider audience.
8. **Multiple Modes of Input**: Players can use mouse, touch, or keyboard controls, improving accessibility and efficiency.
9. **Help and Documentation**: A tutorial popup explains how to play the game, reducing the learning curve.
10. **Feedback and Evaluation**: A post-game summary helps players reflect on their performance.

## 6. Screenshots

(Add screenshots of the game interface, health bar, color-blind mode, tutorial popup, and post-game summary here.)
