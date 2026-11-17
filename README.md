# Retro Bowl College Career Mode

This project includes the compiled Retro Bowl College browser game and a high-school career integrated into its native GameMaker UI. Start a new Player career to create a character, choose Hampshire High or Lavticit High, select QB or RB, and choose a starting rating from 1 to 3 stars. Play a six-game high-school season using the regular on-field gameplay, custom school identities and uniforms, and a Player-specific season screen. After the season, choose between two college offers; the selected offer determines the reduced college-entry rating and initial college attributes.

The Coach option starts directly in FullGame: a 105-player college roster with a position-weighted depth chart, paged roster browsing, benching, higher injury risk, tougher team ratings, and live substitutions. During a match, use the on-field **SUB** button between plays to choose from up to two healthy reserves at each position; simulated results also account for healthy reserve depth. FullGame unlocks the existing team editor in the Options menu so you can change the team name and colors. Exhibition remains available from the main menu and defaults to local two-human pass-and-play.

The career flow uses the game's native UI and in-canvas message system; no browser overlay or separate career storage is used. Player mode skips the introductory tutorial and displays high-school opponents and schedule details instead of the college league during the season. In an RB career, offensive plays hand the ball to the selected player so the normal arrow-key running controls work.

Have Fun!

## Launch

Extract the ZIP, open a terminal in the extracted folder, and run:

```sh
python3 -m http.server 8000
```

Then open `http://localhost:8000/` in your browser. Opening `index.html` directly may leave the game blank because the game loads its assets over HTTP.

## Testing the career modes

Start a new save and choose Player or Coach. Coach now opens FullGame directly. Verify the roster contains 105 players, use the page controls to browse it, bench and reinstate a player, and use **SUB** during a match to choose a healthy reserve. Save and reopen the career to verify persistence. Exhibition can be launched from the main menu; switch both controller selectors to HUMAN for local 1v1 play.
