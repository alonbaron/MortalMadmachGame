# Mortal Madmach

Mortal Madmach is a Java Swing arena fighting game. The player controls one fighter while an AI opponent moves, attacks, defends, and uses special attacks. The game includes character selection, a launcher screen, a how-to-play screen, round scoring, potions, sound effects, custom art, and a win screen.

## Features

- Java Swing desktop game with a fixed 1080x720 window
- Character selection for Boris and Dvora
- Player-vs-AI arena combat
- Health bars and special attack meters
- Basic AI movement, attack, defense, and special-attack behavior
- Health and special potions that spawn during play
- Round system: first fighter to 3 round wins takes the match
- Pause menu, restart/resume flow, and win screen
- Custom image and sound assets bundled under `src/main/resources`

## Controls

| Key | Action |
|---|---|
| Left Arrow | Move left |
| Right Arrow | Move right |
| `Q` | Basic attack |
| `E` | Hold to defend |
| `R` | Special attack |
| `Esc` | Pause / resume |

Developer/debug controls currently present in the game:

| Key | Action |
|---|---|
| `X` | Damage player 1 |
| `C` | Heal player 1 |
| `V` | Fill special meter |

## Tech Stack

- Java 23
- Maven
- Swing / AWT

## Run

Compile the project:

```bash
mvn test
```

Run the game from an IDE by launching:

```text
org.example.Main
```

Or run with Maven's exec plugin:

```bash
mvn compile exec:java -Dexec.mainClass=org.example.Main
```

## Project Structure

```text
src/main/java/org/example/
  Main.java
  GameManager.java
  GamePanel.java
  Player.java
  CharacterSelectPanel.java
  LauncherPanel.java
  HowToPlayPanel.java
  PausePanel.java
  WinPanel.java

src/main/resources/
  images/
  sounds/
```

## Notes

This is a student game project polished for portfolio presentation. The code keeps the original gameplay architecture while making setup and repository intent clearer for readers.

## License

MIT License. See [LICENSE](LICENSE).
