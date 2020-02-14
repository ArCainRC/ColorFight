# ColorFight

This project was for UCLA's Colorfight AI competition, in which teams came up with strategies to gather up most gold in 500 turns, with each game consisting of 4 to 8 players. Link to the description of the rules are on https://colorfightai.com/.

## Strategy ##
Our algorithm was based upon a greedy method, which prioritized *early board domination* by maximizing energy production per turn and taking over other team's territories. (It is a rushing strategy which maximizes early game leads and does poorly in late game).

The algorithm was divided in to 2 stages, with early stage and barrier stage (after turn 40). It would aim to outnumber the energy production per second in first 40 turns, and would aim to attack nearby players with little defense each turn afterwards. It would then place barriers to make teams harder to regain their lost territories.

This bot performed best in a game with many players spawned near each other due to its early game agression. 
Zero Gold mines were placed by this bot after the first game.

## Results ##
This bot placed 4th in the competition, due to its lack of late-game strategies against the lower number of players in the final round (the AI was optimized to shark players in the early game, which was harder to do with less people).

## File Information ##
final_ai.py is the final version of our AI, with the folder Experimental Designs having previous versions of the AI. Segfault 1 and Segfault 2.cfr are replay files showing our AI in action during the matches it won (our team name was Segfault). These replays can be viewed by visiting https://colorfightai.com/replay/local, choosing the "Load Replay" option, and selecting the .cfr file.

### Contributors ###
 - @PranavARC - Algorithm/Function Designer
 - @hyounjunchang - Tester/Experimenter
 - @IanWildenhein - Developer/Code Writer
