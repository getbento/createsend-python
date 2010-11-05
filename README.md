# createsend

A python wrapper for the createsend API v3.

## Installation

    git clone git://github.com/jdennes/createsend-python.git
    cd createsend-python
    python setup.py install

## Example

    from createsend import *
    
    CreateSend.api_key = 'your_api_key'

    cs = CreateSend()
    clients = cs.clients()
    
    for c in clients:
      print "%s: %s" % (c.ClientID, c.Name)
    
    4a397ccaaa55eb4e6aa1221e1e2d7122: Client One
    a206def0582eec7dae47d937a4109cb2: Client Two
