# Control a PLC using WhatsApp

This project demonstrates how to control a Siemens S7-1200 PLC using WhatsApp messages through Node-RED. By setting up a communication flow between WhatsApp and the PLC, you can send commands to the PLC to perform various actions.

## Table of Contents
- [Prerequisites](#prerequisites)
- [Setup](#setup)
  - [PLC Configuration](#plc-configuration)
  - [Node-RED Setup](#node-red-setup)
- [Usage](#usage)
- [Contributing](#contributing)
- [License](#license)

## Prerequisites

Before you begin, ensure you have the following:
- Siemens S7-1200 PLC
- Node-RED installed on your machine
- WhatsApp account
- WhatsApp Web client setup on your machine
- Siemens S7-1200 Node-RED nodes installed

## Setup

### PLC Configuration

1. **Program the PLC:**
   - Set up communication protocols.
   - Define input and output variables.
   - Create a logic program to handle commands from Node-RED.

### Node-RED Setup

1. **Install Node-RED:**
   Follow the instructions to install Node-RED on your machine from the [official Node-RED website](https://nodered.org/docs/getting-started/installation).

2. **Install Siemens S7-1200 Node-RED Nodes:**
   Use the Node-RED palette manager to install the Siemens S7-1200 nodes. Search for `node-red-contrib-s7` and install it.

3. **Import Node-RED Flow:**
   Import the provided `flow.json` file into Node-RED. This flow listens for incoming WhatsApp messages, parses them, and sends the appropriate commands to the PLC.

4. **Configure Siemens S7-1200 Nodes:**
   Configure the Siemens S7-1200 nodes in your Node-RED flow. Set up the Siemens S7-1200 credentials and configure the nodes to communicate with the correct input and output variables in the PLC.

## Usage

1. **Start Node-RED:**
   Run Node-RED on your machine using the command `node-red`.

2. **Open Node-RED:**
   Open the Node-RED editor by navigating to `http://localhost:1880` in your web browser.

3. **Deploy the Flow:**
   Deploy the imported flow to start listening for WhatsApp messages.

4. **Send WhatsApp Messages:**
   Use WhatsApp to send messages like "Green on", "Green off", "Red on", "Red off", etc., to control the PLC.

## Contributing

Contributions are welcome! Please open an issue or submit a pull request for any changes or enhancements.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
