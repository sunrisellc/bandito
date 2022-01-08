Bandito Core integration/staging tree
=====================================

https://www.banditocoin.com

What is Bandito?
----------------
Bandito is a brand new, scrypt based cryptocurrency forked from Litecoin 
and branded for the Bandito Boys(TM), Abner Vaca and Kirk Jerkems of NoPixel.

I've done this as something of a weekend project to keep my skills sharp and will
work on and maintain it pretty much at my leisure. If people show any real
interest or it picks up any type of traction, I may pay it more attention.

In any case, enjoy and have fun!!

Network Difficulty Explained

Difficulty automatically readjusts ever 1008 blocks.
The hard-coded difficulty readjustment target is every 1.75 days.
The hard-coded block generation target is 1 block every 2.5 minutes.

Diff Readustment Target:
“consensus.nPowTargetTimespan = 1.75 * 24 * 60 * 60;” = 151,200 seconds OR 1.75 Days

Block Generation Target:
“consensus.nPowTargetSpacing = 2.5 * 60;” = 150 seconds OR 2.5 Minutes

The Math:
151,200 / 150 = 1008

So… what all of that means is this:

If it takes LESS then 1.75 days for network miners to produce 1008 blocks,
difficulty with be INCREASED based on the recent network hashrate in an attempt
to achieve the desired 1008 blocks per 1.75 days.

If it takes MORE then 1.75 days for network miners to produce 1008 blocks,
difficulty with be REDUCED based on the recent network hashrate in an attempt
to achieve the desired 1008 blocks per 1.75 days.

Network difficulty dictates how difficult it is for a given miner to produce new coins.
As network hashrate is increased, difficulty is as well, making it more difficult to
produce new coins for the network.

It is important to keep this in mind when deciding to add additional hashpower to network.

You may mine more coins, but in the long run without wide, longterm and decentralized support from
miners the network may stall and become unable to process blocks, killing the coin.


(Generic Crypto README.md stuff below)

Bandito is an experimental digital currency that enables instant payments to
anyone, anywhere in the world. Bandito uses peer-to-peer technology to operate
with no central authority: managing transactions and issuing money are carried
out collectively by the network. Bandito Core is the name of open source
software which enables the use of this currency.

For more information, as well as an immediately useable, binary version of
the Bandito Core software, see [https://www.banditocoin.com](https://www.banditocoin.com).

License
-------

Bandito Core is released under the terms of the MIT license. See [COPYING](COPYING) for more
information or see https://opensource.org/licenses/MIT.

Development Process
-------------------

The `master` branch is regularly built and tested, but is not guaranteed to be
completely stable. [Tags](https://github.com/sunrisellc/bandito/tags) are created
regularly to indicate new official, stable release versions of Bandito Core.
