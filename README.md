# Pychain Ledger

This application is a user-friendly decentralized blockchain ledger. This ledger allows banks to make transactions (send and receive money) confidently thruogh hashed information. There is a  button for validating the ledger to verify the integritiy of the data. 




## 1. Import neccessary libraries
```
import streamlit as st
from dataclasses import dataclass
from typing import Any, List
import datetime as datetime
import pandas as pd
import hashlib
```


## 2. Add class **Record**
This class will include 'sender', 'receiver', and 'amount'

## 3. Add class **Block**
This class formats the block. This will include class Record, creater_id, prev_hash, timestamp, and nonce. Hashing the block is part of this step. 

## 4. Add class **Chain**
This step chains all the blocks and includes:
- 'proof_of_work' : adds different difficulty levels of hashing and also adds a *nonce* method.
- 'add_block' : adds the block
- 'is_valid' : checks the validity of the ledger

## 5. Add a Streamlit Interace 
- add an input for sender, receiver, amount, and the button for "Add Block".
- add a sidebar for difficulty
- add a button for validating the information

# Streamlit 
Store transaction record and see the ledger add each block. 
Example of our ledger:
!(Example of ledger){}
