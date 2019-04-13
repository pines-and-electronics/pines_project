# Pines and Electronics

## Components

### Blockchain smart contract

*Running in Rinkeby Ethereum testnet* 

Is a very simple event echo: 

```solidity
contract CarController {
    event CarCommandSent(
        string _command
    );

    function sendCommand (string memory _command)
        public
        returns (bool commandSent)
    {

        emit CarCommandSent(
            _command
        );

        return true;
    }

}
```

### Command listener

*Running in laptop*

Command listener listens to the following strings:
* 'status'
* 'snap'
* 'register'
* 'snapshot'
* 'linear'
* 'steer'

Command listen
        

## Proof of concept

### 1) DAPP

1. User will click on the joystick, and send a string to the 
