
# Mesh Routing Protocol for LoRa

This repository contains the code for implementing a mesh routing protocol for LoRa. 

## Overview

The code uses the RadioHead library to implement a mesh network protocol for LoRa radios. It is designed to work with any number of nodes in the network. The protocol supports sending and receiving messages between nodes, with automatic routing and re-routing in case of node failures.

## Key Features

- **EEPROM Storage**: The node ID is stored in EEPROM, allowing it to be remembered between power cycles.
- **Error Handling**: The code includes a function to return human-readable error messages for various failure modes.
- **Flexible**: The code is designed to work with any number of nodes, defined by the `N_NODES` constant.
- **Routing Table**: After each transmission, the routing table is printed to the serial console for debugging purposes.

## Usage

1. Define the number of nodes in your network with the `N_NODES` constant.
2. Set the node ID for each node. This is stored in EEPROM and remembered between power cycles.
3. Upload the sketch to your Arduino board.

## Dependencies

-  RadioHead Library
  [http://www.airspayce.com/mikem/arduino/RadioHead/]
