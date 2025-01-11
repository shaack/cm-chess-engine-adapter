# cm-engine-runner

A JavaScript module to act as a framework for running chess engines in the browser.

## Working engines

### Stockfish 10

- File: `engines/stockfish-v10-niklasf.js`
- Type: WebWorker
- Stockfish version: 10
- Latest Version with WebWorker
- https://github.com/niklasf/stockfish.js

### Polyglot opening books

- An engine to play moves from a polyglot (.bin) openings file.
- https://github.com/shaack/cm-polyglot

### Stockfish 14

Not implemented yet, does not work in Safari as of 2021-12-12

- Type: WASM
- Stockfish version: 14
- Latest js version, multithreaded
- https://github.com/nmrugg/stockfish.js

## Stockfish Skill Levels

    this.uciCmd('setoption name Skill Level value ' + (LEVELS[props.level][1]))

- Level 0 = 1100 ELO rating
- Level 1 = 1165 ELO rating
- Level 2 = 1230 ELO rating

As you can see the strength is increasing by 65 ELO points for each level, so that;

- Level 20 = 2570 ELO rating.

And depth to ELO: https://chess.stackexchange.com/questions/8123/stockfish-elo-vs-search-depth?rq=1

## References

- [UCI reference](http://page.mi.fu-berlin.de/block/uci.htm)
- [Official Stockfish](https://github.com/official-stockfish/Stockfish)
- [stockfish.js](https://github.com/nmrugg/stockfish.js/)
  - https://github.com/mcostalba/Stockfish
  - https://github.com/niklasf/stockfish.js (stockfish-v10-niklasf.js)
  - https://github.com/bjedrzejewski/stockfish-js <= supports opening books
- [chess-tools](https://github.com/johnfontaine/chess-tools)
- https://www.chessprogramming.org/Opening_Book#Formats 
- https://github.com/evilwan/stakelbase

---

Find more high quality JavaScript modules from [shaack.com](https://shaack.com)
on [our projects page](https://shaack.com/works).
