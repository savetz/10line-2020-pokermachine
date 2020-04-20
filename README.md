# 10line-pokermachine
Poker Machine game in Turbo BASIC XL for Atari 8-bit. Entry for 2020 10-line BASIC contest

My first entry for the 2020 10-line BASIC contest is a poker machine simulator written in TurboBASIC XL for the Atari 8-bit computer. At ten 120-character lines, it qualifies for the PUR-120 category. It is based on the common “Jacks Or Better” poker machine, although I changed the payouts to make it more fun and to conserve space.

The game deals a hand of five playing cards. You can choose to “hold” any or all of the cards by pressing 1 though 5, then press any other key to replace the cards that you did not hold. (Held cards are not replaced.) It then calculates whether you’ve won, based on standard poker hands.

Here are the payouts:

royal flush +650 (real game: 1250)
royal straight +500 (not in real game)
straight flush +350 (real game: 250)
4 of a kind +225 (real game: 125)
full house +150 (real game: 30)
flush +150 (real game: 25)
straight +200 (real game: 20)
3 of a kind +150 (real game: 15)
2 pair +50 (real game: 10)
pair of Jacks or better +5 (real game: 10)

With all the logic for calculating poker hands, there wasn’t room for card graphics. I did make a custom character set with just one special character: a “10” for the only two-digit card. I am proud of squeezing in money though. You start with $50 in your wallet, and the game costs $5 per hand. The game remembers your wallet by poking it into unused memory ($600, the top of Page 6) then peeking it back after it re-RUNs. Because RUN clears all the variables, this uses much less program space than resetting all the variables by hand.
