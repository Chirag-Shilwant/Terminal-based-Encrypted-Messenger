# Terminal based Encrypted Messenger

- A Terminal based Encrypted Messenger. 
- To ensure secure communication the messages are encrypted using **Triple DES(3DES)** which is a Symmetric Encryption technique and the secret key used for encryption will be exchanged between the users using **Diffie–Hellman key exchange algorithm**.

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
- The message is encrypted using **Tripple DES (3DES)** which is a Symmetric Encryption Technique and the secret key exchange algorithm used between the users is **Diffie–Hellman**.
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
