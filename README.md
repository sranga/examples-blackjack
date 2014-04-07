Simple Blackjack App
====================

Simple implementation of the Blackjack game. The assumptions made and functionality supported follow.

Assumptions:
------------
The game starts by dealing out two cards each to the player and dealer. A score of 21 wins the game for the player or dealer.
In the event of a tie, the dealer wins. The user shall receive ***100*** coins at the beginning of the game.
He can choose to bet any number of available coins at each hand. Once all the coins are exhausted, the game ends.
The user can choose to **Hit** by entering a **H** when prompted. A **S** response would be assumed to be a **Stand**.

Requirements:
-------------
* SBT 0.13.1 - [Install](http://www.scala-sbt.org/release/docs/Getting-Started/Setup.html)
* Scala 2.10.3+ - [Install](http://www.scala-lang.org/download/2.10.3.html)
* Java 1.7+ - [Install](http://www.oracle.com/technetwork/java/javase/downloads/jdk7-downloads-1880260.html)

Usage:
------
* Checkout the codebase: `git clone https://github.com/sranga/examples.git`
* This project requires SBT to build and run. Please download and install it using this page: [SBT Setup](http://www.scala-sbt.org/release/docs/Getting-Started/Setup.html)
* After SBT is successfully installed, start the game using `sbt run` from the *examples* (top-level) directory

Sample Output:
--------------
    Welcome to the Single-user BlackJack game!
    ------------------------------------------
    The game starts by dealing out two cards each to the player and dealer. A score of 21 wins the game for the player or dealer.
    In the event of a tie, the dealer wins. The user shall receive 100 coins at the beginning of the game.
    He can choose to bet any number of available coins at each hand. Once all the coins are exhausted, the game ends.
    The user can choose to "Hit" by entering a "H" when prompted. A "S" response would be assumed to be a "Stand".
    Good Luck!!


    ---------------- Starting New Hand ----------------

    Please enter your bet for this round. Credit at hand: [ 100 ]
    10
    Bet for the current hand: ( 10 )

    Dealer hand: [ 10 X ]
    Player hand: [ 2, 8 ]

    Hit or Stand? Enter one of (H,h,S,s): h
    Dealer hand: [ 10 X ]
    Player hand: [ 2, 8, 10 ]

    Hit or Stand? Enter one of (H,h,S,s): s
    *** You win! ***
    Dealer hand: [ 10, 7 ]
    Player hand: [ 2, 8, 10 ]

    Continue the game? Enter one of (Y,y,N,n): y

    ---------------- Starting New Hand ----------------

    Please enter your bet for this round. Credit at hand: [ 110 ]
    50
    Bet for the current hand: ( 50 )

    Dealer hand: [ 10 X ]
    Player hand: [ 2, 8 ]

    Hit or Stand? Enter one of (H,h,S,s): h
    Dealer hand: [ 10 X ]
    Player hand: [ 2, 8, 10 ]

    Hit or Stand? Enter one of (H,h,S,s): s
    *** You lose! ***
    Dealer hand: [ 10, 10 ]
    Player hand: [ 2, 8, 10 ]

    Continue the game? Enter one of (Y,y,N,n): y

    ---------------- Starting New Hand ----------------

    Please enter your bet for this round. Credit at hand: [ 60 ]
    60
    Bet for the current hand: ( 60 )

    Dealer hand: [ 10 X ]
    Player hand: [ 2, 1 ]

    Hit or Stand? Enter one of (H,h,S,s): h
    Dealer hand: [ 10 X ]
    Player hand: [ 2, 1, 6 ]

    Hit or Stand? Enter one of (H,h,S,s): h
    Dealer hand: [ 10 X ]
    Player hand: [ 2, 1, 6, 5 ]

    Hit or Stand? Enter one of (H,h,S,s): h
    Dealer hand: [ 10 X ]
    Player hand: [ 2, 1, 6, 5, 5 ]

    Hit or Stand? Enter one of (H,h,S,s): h
    *** You lose! ***
    Dealer hand: [ 10, 2 ]
    Player hand: [ 2, 1, 6, 5, 5, 9 ]


    ======= Game Summary =======
    Start-Credit: [ 100 ],  End-Credit: [ 0 ]
    Round: 1, Result: Won, Player: [ 2, 8, 10 ], Dealer: [ 10, 7 ]
    Round: 2, Result: Lost, Player: [ 2, 8, 10 ], Dealer: [ 10, 10 ]
    Round: 3, Result: Lost, Player: [ 2, 1, 6, 5, 5, 9 ], Dealer: [ 10, 2 ]