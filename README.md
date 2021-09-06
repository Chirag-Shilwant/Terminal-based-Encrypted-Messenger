# An end to end messaging system like WhatsApp

## How to run

    pip3 install pycryptodome
    run server: ./server.py
    run client: ./client.py PORT


## Features
- Multiclient chat application that has a server component and atleast 4 clients.
- The system supports the signup and sign in feature. [error message with wrong credentials].
- User can send message to other user [p2p message] [ SEND command] [<SEND><USERNAME><MESSAGE>]
- Each user can join multiple chat rooms (groups) at a time.
- Each user can list all the groups.  [LIST Command] [show all group and number of participants ineach group]
- Each user can join a group [JOIN command]. If the group does not exist then the first create it thenjoins it.
- Each user can create a group [CREATE command].
- If one user sends a message to a group it should be sent to all members of that group.
- The message is encrypted using **Tripple DES (3DES)** and the key exchange algorithm used between clients is **Diffie–Hellman**. Each group has one key (random nonce).
- Each group has one key (random nonce).
- **Message can be any type, for example, text, images, video, and audio.**

## Commands Implemented
    1. create_account
    2. login
    3. create_group
    4. list_groups
    5. join_groups
    6. Peer to peer(p2p) text messaging
    7. group messaging
    8. p2p file sharing
    9. group file sharing
