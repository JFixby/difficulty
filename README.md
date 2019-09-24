[![Build Status](https://travis-ci.org/jfixby/difficulty.png?branch=master)](https://travis-ci.org/jfixby/difficulty)
[![ISC License](http://img.shields.io/badge/license-ISC-blue.svg)](http://copyfree.org)
[![GoDoc](https://img.shields.io/badge/godoc-reference-blue.svg)](http://godoc.org/github.com/jfixby/difficulty)
[![Go Report Card](https://goreportcard.com/badge/github.com/jfixby/difficulty)](https://goreportcard.com/report/github.com/jfixby/difficulty)

# Difficulty

 Difficulty is a struct modeling the concept of how difficult it is to find a hash below a given target (https://en.bitcoin.it/wiki/Difficulty)
 
 
  Difficulty supports three different representations:
  
  1) Hex string
  
       example: `00000000ffffffffffffffffffffffffffffffffffffffffffffffffffffffff`
       
  2) big.Int
  
       example: `new(big.Int).Sub(new(big.Int).Lsh(bigOne, 256-32), bigOne)`
       
  3) Bits, or in a compact form
  
       example: `0x1d00ffff`
