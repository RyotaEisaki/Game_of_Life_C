# Conway's Game of Life
[Wikipedia](https://en.wikipedia.org/wiki/Conway%27s_Game_of_Life)


　ライフゲーム (Conway's Game of Life) は1970年にイギリスの数学者ジョン・ホートン・コンウェイ (John Horton Conway) が考案した生命の誕生、進化、淘汰などのプロセスを簡易的なモデルで再現したシミュレーションゲームである。単純なルールでその模様の変化を楽しめるため、パズルの要素を持っている。



生物集団においては、過疎でも過密でも個体の生存に適さないという個体群生態学的な側面を背景に持つ。セル・オートマトンのもっともよく知られた例でもある。 


 The Game of Life, also known simply as Life, is a cellular automaton devised by the British mathematician John Horton Conway in 1970.


The game is a zero-player game, meaning that its evolution is determined by its initial state, requiring no further input. One interacts with the Game of Life by creating an initial configuration and observing how it evolves, or, for advanced players, by creating patterns with particular properties. 

## Rules

　ライフゲームでは初期状態のみでその後の状態が決定される。碁盤のような格子があり、一つの格子はセル（細胞）と呼ばれる。各セルには8つの近傍のセルがある (ムーア近傍) 。各セルには「生」と「死」の2つの状態があり、あるセルの次のステップ（世代）の状態は周囲の8つのセルの今の世代における状態により決定される。

セルの生死は次のルールに従う。

* **[誕生] 死んでいるセルに隣接する生きたセルがちょうど3つあれば、次の世代が誕生する。**
    
* **[生存] 生きているセルに隣接する生きたセルが2つか3つならば、次の世代でも生存する。**

* **[過疎] 生きているセルに隣接する生きたセルが1つ以下ならば、過疎により死滅する。**

* **[過密] 生きているセルに隣接する生きたセルが4つ以上ならば、過密により死滅する。**
    

 The universe of the Game of Life is an infinite, two-dimensional orthogonal grid of square cells, each of which is in one of two possible states, alive or dead, (or populated and unpopulated, respectively). Every cell interacts with its eight neighbours, which are the cells that are horizontally, vertically, or diagonally adjacent. At each step in time, the following transitions occur:

* **Any live cell with fewer than two live neighbours dies, as if by underpopulation.**
* **Any live cell with two or three live neighbours lives on to the next generation.**
* **Any live cell with more than three live neighbours dies, as if by overpopulation.**
* **Any dead cell with exactly three live neighbours becomes a live cell, as if by reproduction.**

The initial pattern constitutes the seed of the system. The first generation is created by applying the above rules simultaneously to every cell in the seed; births and deaths occur simultaneously, and the discrete moment at which this happens is sometimes called a tick. Each generation is a pure function of the preceding one. The rules continue to be applied repeatedly to create further generations. 

## Source Code
[Click Here](https://github.com/RyotaEisaki/Game_of_Life_C/blob/master/game_of_life.c)

## Input

　[入力](https://github.com/RyotaEisaki/Game_of_Life_C/blob/master/ex_input1)は次のような形をしている。
```
10
10
O . . . . . . . O O
. O . . . . . . O O
. . O . . . . . . .
. . . O . . . . . .
. . . O O . . . . .
. . O O O O . . . .
. O O O O O O . . .
O O O O O O O O . .
. . . . . . . . O .
. . . . . . . . . O
5
```

