## Project Overview

This project, titled "Module 1: Create Blockchain," is a basic implementation of a blockchain using Python. The code includes functionalities to create new blocks, validate the integrity of the blockchain, and perform proof-of-work calculations.
Features

# Blockchain Class: A core class that manages the blockchain operations.
# Block Creation: Functionality to add new blocks to the chain with a timestamp, proof, and the hash of the previous block.
# Proof of Work: An algorithm to ensure computational work has been done to add a new block.
# Chain Validation: Checks the integrity of the blockchain to ensure data hasn't been tampered with.

# Requirements

    Python 3.x
    Flask
    hashlib
    datetime
    json

## API Endpoints

    /create_block: To create a new block.
    /get_chain: To retrieve the current blockchain.
    /is_valid: To check if the blockchain is valid.

## How it Works

    Initialization: When the Blockchain class is instantiated, it creates the genesis block.
    Adding Blocks: New blocks are added by providing a proof of work and the hash of the previous block.
    Proof of Work: A simple algorithm that finds a number such that when hashed with the previous proof, the hash starts with four leading zeroes.
    Validation: The integrity of the chain is checked by ensuring that each block's previous hash matches the hash of the previous block and that the proof of work is valid.
