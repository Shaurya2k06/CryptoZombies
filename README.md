# CryptoZombies

CryptoZombies is a Solidity-based project designed to teach blockchain development through the creation of a zombie-themed game. The project demonstrates key concepts of smart contract development, including inheritance, mappings, structs, and external contract interactions.

## Project Structure

### Files
1. **zombiefactory.sol**  
   This file contains the `ZombieFactory` contract, which is responsible for creating and managing zombies. It includes:
   - Zombie struct definition.
   - Functions for generating random DNA and creating zombies.
   - Mappings to track zombie ownership.

2. **zombiefeeding.sol**  
   This file contains the `ZombieFeeding` contract, which inherits from `ZombieFactory`. It introduces:
   - Interaction with an external `KittyInterface` contract.
   - Functions to feed zombies and mutate their DNA based on external inputs.

3. **README.md**  
   This file (you are reading it) provides an overview of the project.

### Key Concepts
- **Inheritance**: The `ZombieFeeding` contract inherits from `ZombieFactory`.
- **External Contract Interaction**: The `ZombieFeeding` contract interacts with the `KittyInterface` to fetch data from another smart contract.
- **Mappings**: Used to track ownership of zombies and count the number of zombies owned by an address.

## How It Works
1. Users can create a random zombie using the `createRandomZombie` function in `ZombieFactory`.
2. Zombies can feed on other entities (e.g., CryptoKitties) using the `feedOnKitty` function in `ZombieFeeding`.
3. Feeding results in the creation of a new zombie with DNA derived from the parent zombie and the target entity.

## Prerequisites
- Solidity version `>=0.5.0 <0.6.0`.
- A basic understanding of smart contracts and Ethereum blockchain.

## Future Enhancements
- Add more interactions between zombies and other entities.
- Implement a battle system for zombies.
- Introduce additional external contract integrations.

## License
This project is for educational purposes and does not include a specific license. Feel free to use and modify it as needed.