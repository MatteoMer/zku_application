# ZK University application
Application for the [ZK University](https://zku.one/apply-now) by Harmony

## Questions
1. **What is a hash? Why do people use hashing to hide information?**
    A hash is a function (most of the time an mathematical algorithm) that computes what could be described as the program (or any file/string) "signature".
    This signature is unique for each program and we cannot get the file from the signature (it's only one way).

    People use hashing to hide informations since it allows to check if an information is true without revealing the information.
    Simple example: We don't want to store passwords in a database, since it could be hacked. 
    We instead store an hash of the password, and when an user is logging in, we compute the hash of the password given by user, and then compare it with the one in the database. If they match, we can allow the user to login!

2. **What is a smart contract?**
    First, a smart contract could be defined as some code that will run deterministically in the EVM (for Ethereum).
    It is a contract because it's an agreement between multiples parties that for a define event happening, a defined outcome will occur,
    and it's smart because the contract doesn't need any human action to have his terms respected. If in the contract event a creates outcome b, then in a smart contract, if event a happens, outcome b will always happen (automatically).
    This contract is run by different computers (nodes) to make sure the result is right, and also can be verified (because it's not centralized in one place)
    Technically, a smart contract is a bytecode, that, when is translated in a more human-readable way, use opcodes to change the state of the blockchain, do basic operations (additions, multiplications, etc..) as well as a lot more different call that could be useful to write a contract!


3. **What are gas fees? Why is gas optimization a big focus when building smart contracts?**
    Gas is how much cost a computation to run a decentralized blockchain, it's used to pay the miners that run the computations of the contract!
    All the opcodes (described before) have a fixed gas cost, and we need to add all of the gas gost to have our total gas price, that the user will need to pay to have his transaction validated.
    Gas optimization is a big focus because since the user is paying for the gas, if we're doing over-complicated stuff in our contract, the user will pay more gas (and gas can be super expensive!)
    If we want to have more user using our product more, we need to optimize gas to make an app more affordable

4. **You have the ability to quickly count the number of leaves in a tree. How can you prove this to a friend, without revealing the exact number of leaves?**
    First, I'll ask my friend to choose a tree, I will count the number of leaves in this tree and keep it for me.
    Then I will close my eyes and ask my friend to remove a random number of leaves on this tree (and hide/destroy them).
    I will count the number of leaves again and will substract it from the initial number. 
    Now I have the number of leaves that my friend removed and it's a proof that I know how much leaves are on this tree!
    With one tree, it could be luck, so we could do this again and again with differents trees to build confidence that I know the result.

