[![License: CC BY-NC-SA 4.0](https://img.shields.io/badge/License-CC%20BY--NC--SA%204.0-lightgrey.svg)](https://creativecommons.org/licenses/by-nc-sa/4.0/)

Partially Non-Interactive and Instantaneous Bitcoin One-way Payment Channel
===

[Paper](./btc-channel.pdf)

## Abstract

The most significant challenge for Bitcoin in the coming years
is scalability. Currently, Bitcoin enforces a 1 Megabyte block-size limit. On
average every 10 minutes a new block is discovered. That produces a payment
network limited to $\approx7$ transactions per second, and with delayed (and
unknown) transaction confirmation times. This is not sufficient in comparison
to the currently deployed payment infrastructure such as credit card
processors, which allows tens of thousands of transactions per second. To
address this, there are some proposals to modify (i) the transaction structure
(such as in SegWit), (ii) the block-size limit (such as SegWit2x) or even
(iii) build a second layer on top of the Bitcoin protocol (such as the
Lightning Network). Following the rational of second layer solutions, we
propose a retail-ready, one-way payment channel that enables two parties to
transact mostly off-chain, thus reducing the number of on-chain transactions
and operational cost, while remaining secure and trustless. After the channel
is opened for a few blocks, payment channel transactions are instantaneous and
irreversible, and do not rely on the seemly random block arrival times. At all
times, only one of the parties (the money receiver) must stay online to secure
the channel integrity. The money receiver can redeem his channel funds on
chain with no delay at all times. The money sender does not have to perform
any action to secure its funds.

## Building LaTex

A `Makefile` is provided to compile the project, just use `make`

About
===

Authors: Thomas Shababi, Joel Gugger, and Daniel Lebrecht. Copyright (C) TrueLevel SA, Joel Gugger, Daniel Lebrecht.
