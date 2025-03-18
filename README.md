twamp-protocol
==============

A Two-Way Active Measurement Protocol

Read the RFC:
    http://tools.ietf.org/html/rfc5357

Source Repository:
    https://github.com/emirica/twamp-protocol.git  
Developer:
    Emma Mirică  
Contributions:
    stephanDB

Patches Repository:
    https://github.com/fnoobt/twamp-protocol.git 
Contributions:
    fnoobt

Note:
    This is a minimal implementation of the TWAMP protocol.

    What is Newly Supported:
        - Client and server support IPv6 addresses
    
    What is not supported:
        - the authenticated, encrypted mode for client and server
        - it has the option to set this mode for client and server, but is not
          yet supported. The messages were defined but the logic is not
          implemented.

    To run:
        make
        make setcap
        ./server [-h | -a <not supported> | -p <port>]
        ./client -s <ip_server [-h | -a <not_supported> | -p <port_sender> | -P
        <port_receiver> | -n <test_sessions> | -m <test_sess_msgs>]
