# FavoriteRecords

Record management system with nested mappings for tracking user preferences on approved albums.

## Description

This contract manages a curated list of approved music records and allows users to maintain their personal favorites list. It uses nested mappings to efficiently track user preferences and includes validation to ensure only approved records can be added.

## Features

- **Approved Records List**: Pre-loaded with 9 classic albums
- **User Favorites**: Personal favorites list for each user
- **Nested Mappings**: Efficient storage using `mapping(address => mapping(string => bool))`
- **Custom Error Handling**: Specific error for unapproved albums

## Pre-loaded Albums

1. Thriller
2. Back in Black
3. The Bodyguard
4. The Dark Side of the Moon
5. Their Greatest Hits (1971-1975)
6. Hotel California
7. Come On Over
8. Rumours
9. Saturday Night Fever

## Deployment Instructions

1. Open [Remix IDE](https://remix.ethereum.org/)
2. Create a new file and copy-paste the contract code
3. Compile the contract using Solidity ^0.8.0
4. Deploy on **Base Sepolia Testnet**
5. Interact with the functions:
   - `getApprovedRecords()` - View all approved albums
   - `addRecord(string albumName)` - Add album to your favorites
   - `getUserFavorites(address user)` - Get user's favorite albums
   - `resetUserFavorites()` - Clear your favorites

## Submit Exercise

[📖 Submit Mappings Exercise](https://docs.base.org/learn/mappings/mappings-exercise)
