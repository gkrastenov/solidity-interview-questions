# Solidity Interview Questions

Over 140 interview questions for Ethereum Developers
All of these questions can be answered in three sentences or less.

# Easy
1. What is the difference between private, internal, public, and external functions?

2. Approximately, how large can a smart contract be?

3. What is the difference between create and create2?

4. What major change with arithmetic happened with Solidity 0.8.0?

5. What special CALL is required for proxies to work?

6. Prior to EIP-1559, how do you calculate the dollar cost of an Ethereum transaction?

7. What are the challenges of creating a random number on the blockchain?

8. What is the difference between a Dutch Auction and an English Auction?

9. What is the difference between transfer and transferFrom in ERC20?

10. Which is better to use for an address allowlist: a mapping or an array? Why?

11. Why shouldn’t tx.origin be used for authentication?

12. What hash function does Ethereum primarily use?

13. How much is 1 gwei of Ether?

14. How much is 1 wei of Ether?

15. What is the difference between assert and require?

16. What is a flash loan?

17. What is the check-effects pattern?

18. What is the minimum amount of Ether required to run a solo staking node?

19. What is the difference between fallback and receive?

20. What is reentrancy?

21. As of the Shanghai upgrade, what is the gas limit per block?

22. What prevents infinite loops from running forever?

23. What is the difference between tx.origin and msg.sender?

24. How do you send Ether to a contract that does not have payable functions, or a receive or fallback?

25. What is the difference between view and pure?

26. What is the difference between transferFrom and safeTransferFrom in ERC721?

27. How can an ERC1155 token be made into a non-fungible token?

28. What is access control and why is it important?

29. What does a modifier do?

30. What is the largest value a uint256 can store?

31. What is variable and fixed interest rate?

# Medium
1. What is the difference between transfer and send? Why should they not be used?

2. How do you write a gas-efficient for loop in Solidity?

3. What is a storage collision in a proxy contract?

4. What is the difference between abi.encode and abi.encodePacked?

5. uint8, uint32, uint64, uint128, uint256 are all valid uint sizes. Are there others?

6. What changed with block.timestamp before and after proof of stake?

7. What is frontrunning?

8. What is a commit-reveal scheme and when would you use it?

9. Under what circumstances could abi.encodePacked create a vulnerability?

10. How does Ethereum determine the BASEFEE in EIP-1559?

11. What is the difference between a cold read and a warm read?

12. How does an AMM price assets?

13. What is a function selector clash in a proxy and how does it happen?

14. What is the effect on gas of making a function payable?

15. What is a signature replay attack?

16. What is gas griefing?

17. How would you design a game of rock-paper-scissors in a smart contract such that players cannot cheat?

18. What is the free memory pointer and where is it stored?

19. What function modifiers are valid for interfaces?

20. What is the difference between memory and calldata in a function argument?

21. Describe the three types of storage gas costs.

22. Why shouldn’t upgradeable contracts use the constructor?

23. What is the difference between UUPS and the Transparent Upgradeable Proxy pattern?

24. If a contract delegatecalls an empty address or an implementation that was previously self-destructed, what happens? What if it is a regular call instead of a delegatecall?

25. What danger do ERC777 tokens pose?

26. According to the solidity style guide, how should functions be ordered?

27. According to the solidity style guide, how should function modifiers be ordered?

28. What is a bonding curve?

29. How does safeMint differ from mint in the OpenZeppelin ERC721 implementation? 

30. What keywords are provided in Solidity to measure time?

31. What is a sandwich attack?

32. If a delegatecall is made to a function that reverts, what does the delegatecall do?

33. What is a gas efficient alternative to multiplying and dividing by a multiple of two?

34. How large a uint can be packed with an address in one slot?

35. Which operations give a partial refund of gas?

36. What is ERC165 used for?

37. If a proxy makes a delegatecall to A, and A does address(this).balance, whose balance is returned, the proxy's or A?

38. What is a slippage parameter useful for?

39. What does ERC721A do to reduce mint costs? What is the tradeoff?

40. Why doesn't Solidity support floating point arithmetic?

41. What is TWAP?

42. How does Compound Finance calculate utilization?

43. If a delegatecall is made to a function that reads from an immutable variable, what will the value be?

# Hard
1. How does fixed point arithmetic represent numbers?

2. What is an ERC20 approval frontrunning attack?

3. What opcode accomplishes address(this).balance?

4. How many arguments can a solidity event have?

5. What is an anonymous Solidity event?

6. Under what circumstances can a function receive a mapping as an argument?

7. What is an inflation attack in ERC4626

8. How many arguments can a solidity function have?

9. How many storage slots does this use? uint64[] x = [1,2,3,4,5]? Does it differ from memory?

10. Prior to the Shanghai upgrade, under what circumstances is returndatasize() more efficient than push zero?

11. Why does the compiler insert the INVALID op code into Solidity contracts?

12. What is the difference between how a custom error and a require with error string is encoded at the EVM level?

13. What is the kink parameter in the Compound DeFi formula?

14. How can the name of a function affect its gas cost, if at all?

15. What is a common vulnerability with ecrecover?

16. What is the difference between an optimistic rollup and a zk-rollup?

17. How does EIP1967 pick the storage slots, how many are there, and what do they represent?

18. How much is one Sazbo of ether?

19. What can delegatecall be used for besides use in a proxy?

20. Under what circumstances would a smart contract that works on Etheruem not work on Polygon or Optimism? (Assume no dependencies on external contracts)

21. How can a smart contract change its bytecode without changing its address?

22. What is the danger of putting msg.value inside of a loop?

23. Describe the calldata of a function that takes a dynamic length array of uint128 when uint128[1,2,3,4] is passed as an argument

24. Why is strict inequality comparisons more gas efficient than ≤ or ≥? What extra opcode(s) are added?

25. If a proxy calls an implementation, and the implementation self-destructs in the function that gets called, what happens?

26. What is the relationship between variable scope and stack depth?

27. What is an access list transaction?

28. How can you halt an execution with the mload opcode?

29. What is a beacon in the context of proxies?

30. Why is it necessary to take a snapshot of balances before conducting a governance vote?

31. How can a transaction be executed without a user paying for gas?

32. In solidity, without assembly, how do you get the function selector of the calldata?

33. How is an Ethereum address derived?

34. What is the metaproxy standard?

35. If a try catch makes a call to a contract that does not revert, but a revert happens inside the try block, what happens?

36. If a user calls a proxy makes a delegatecall to A, and A makes a regular call to B, from A's perspective, who is msg.sender? from B's perspective, who is msg.sender? From the proxy's perspective, who is msg.sender?

37. Under what circumstances do vanity addresses (leading zero addresses) save gas?

38. Why do a significant number of contract bytecodes begin with 6080604052? What does that bytecode sequence do?

39. How does Uniswap V3 determine the boundaries of liquidity intervals?

40. What is the risk-free rate?

41. When a contract calls another call via call, delegatecall, or staticcall, how is information passed between them?

# Advanced
1. What addresses to the ethereum precompiles live at?

2. How does Solidity manage the function selectors when there are more than 4 functions?

3. If a delegatecall is made to a contract that makes a delegatecall to another contract, who is msg.sender in the proxy, the first contract, and the second contract?

4. How does ABI encoding vary between calldata and memory, if at all?

5. What is the difference between how a uint64 and uint256 are abi-encoded in calldata?

6. What is read-only reentrancy?

7. What are the security considerations of reading a (memory) bytes array from an untrusted smart contract call?

8. If you deploy an empty Solidity contract, what bytecode will be present on the blockchain, if any?

9. How does the EVM price memory usage?

10. What is stored in the metadata section of a smart contract?

11. What is the uncle-block attack from an MEV perspective?

12. How do you conduct a signature malleability attack?

13. Under what circumstances do addresses with leading zeros save gas and why?

14. What is the difference between payable(msg.sender).call{value: value}(””) and msg.sender.call{value: value}(””)?

15. How many storage slots does a string take up?

16. How does the --via-ir functionality in the Solidity compiler work?

17. Are function modifiers called from right to left or left to right, or is it non-deterministic?

18. If you do a delegatecall to a contract and the opcode CODESIZE executes, which contract 2. size will be returned?

19. Why is it important to ECDSA sign a hash rather than an arbitrary bytes32?

20. Describe how symbolic manipulation testing works.

21. What is the most efficient way to copy regions of memory?

22.  How can you validate on-chain that another smart contract emitted an event, without using an oracle?

23. When selfdestruct is called, at what point is the Ether transferred? At what point is the smart contract's bytecode erased?

24. Under what conditions does the Openzeppelin Proxy.sol overwrite the free memory pointer? Why is it safe to do this?

25. Why did Solidity deprecate the "years" keyword?

26. What does the verbatim keyword do, and where can it be used?

27. How much gas can be forwarded in a call to another smart contract?

28. What does an int256 variable that stores -1 look like in hex?

29. What is the use of the signextend opcode?

30. Why do negative numbers in calldata cost more gas?

31. What is a zk-friendly hash function and how does it differ from a non-zk-friendly hash function?

32. What is a nullifier in the context of zero knowledge, and what is it used for?