# Pines and Electronics

## Components

### 1) Blockchain smart contract (the **DAO**)

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

### 2) DAPP frontent

*Running in a laptop*

Has following buttons:
* Joystick
  * sendCommand()
* Snapshot
  * sendCommand()



### 3) Command listener

*Running in laptop*

Command listener listens to the following strings:
* 'status'
* 'snap'
* 'register'
* 'snapshot'
* 'linear'
* 'steer'



## Proof of concept

### 1) DAPP

1. User will click on the joystick, and send a string to the 
