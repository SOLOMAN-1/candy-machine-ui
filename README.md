# Candy Machine UI Setup Guide

## Overview
This guide provides comprehensive instructions for establishing the user interface (UI) for your Candy Machine. This UI facilitates NFT minting using the SPL token you've generated, with payment processed through the SPL token. Users can seamlessly mint NFTs by linking their Phantom wallets.

## Prerequisites
Ensure you have the following:

- A configured Candy Machine with specific details in its `config.json` file, including pricing, quantity, symbol, seller fee, SPL token account, SPL token, go-live date, and creator details.
- A Phantom wallet designated for minting.

## Steps

### 1. Set Up the SPL Token
If not done already, create the SPL token as per the guidelines in Lesson Three, and make a note of its address.

### 2. Update Candy Machine Config
Modify your Candy Machine's `config.json` file:

- Update `splTokenAccount` with the created SPL token account address.
- Update `splToken` with the SPL token address.

### 3. Set Up the UI
Refer to the "Quick Node: Set Up a Minting Site" tutorial to construct a user-friendly interface for your Candy Machine. This UI enables users to connect their Phantom wallets and mint NFTs, utilizing the SPL token for payment.

### 4. Modify Minting Logic
In your SPL project's minting logic (per Lesson Three), adjust it to mint NFTs to the Phantom wallet address or modify the transfer function to deliver minted NFTs to your Phantom wallet.

### 5. Testing
Thoroughly test your setup by transferring or minting your SPL token to a Phantom account. Utilize the created UI to mint NFTs; users should successfully mint NFTs by paying with the designated SPL token.
