# Sheepy Time — Text-Based Java Game (Solo Mode)

A console-based Java adaptation of *Sheepy Time* by Neil Kimball, created for an Object-Oriented Design (OOD) course.  
The game uses **MVC architecture**, **SOLID principles**, and includes extensive **unit testing** for Models, Views, and Controllers.

## Contributors
- Adil Alimzhanov
- Tan Karageldi
- Derrick Ansah
- Tolga Cohce

## How to Run
Open the project in any Java IDE or terminal and run:

```
Main.java
```

## Game Overview
You play as a dream sheep navigating the dream track while avoiding the Nightmare.  
Your objective is to collect **Winks** before the Nightmare wakes the dreamer.

### Key Resources
- **Zzzs** → Gain abilities  
- **Winks** → Required to win  

### Nightmare Cards
The Nightmare deck dictates enemy movement and special effects each round.

---

## Architecture Overview
### MVC Breakdown
- **Model** — Sheep, Nightmare, Board, Cards, Deck, Abilities  
- **View** — Console output, display helpers  
- **Controller** — Game loop, turn resolution, rule enforcement

### SOLID Principles Used
- **SRP:** Each class handles one domain responsibility  
- **OCP:** New cards/abilities can be added without changing existing logic  
- **LSP:** All `Card` subclasses behave consistently with the `Card` base type  
- **ISP:** No “god interfaces”; responsibilities are separated  
- **DIP:** Controller depends on abstractions (View, Card types)  

---

## Testing
Unit tests were created for:
- Model entities  
- Movement logic  
- Card behaviors  
- Board interactions  
- View rendering  
- Controller flow  

The project includes high test coverage to validate the game loop, card effects, and player/nightmare interactions.

---

## Project Structure
```
src/
 ├── controller/
 ├── model/
 ├── view/
 └── Main.java
```

---

## License
For educational use only. Not affiliated with the official Sheepy Time board game.
