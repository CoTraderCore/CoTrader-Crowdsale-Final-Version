
# Changes
1) add ReduceLimit 

2) add 2B to limit per 90 days

3) add function block pauseTokens

4) add SetLimitAmount Owner can change limit amount for iSLByMAL

5) add more test

# Additional functions

0 ReduceLimit() After call this function owner can not set new limit more than value of parametr previous call

1 ReduceRate()
Owner can reduce bonus percent 25% by default each call reduces of 1%

2 setRLTime() 
Owner can change TimeLimit for IMLimit

3 iSLByMAL()
Owner can ADD 2B to limit, 100B maximum tokens limit
TimeLimit for call by default one time in 90 days

4 blockSetRLTime()
Owner can block setRLTime() forever

5 isSetRLTimeStatus()
View status of setRLTim() function

6 MintLimit() 
Owner can mint new Tokens up to a certain limit 20B minLimit 100B maxLimit Owner can mint only through contract sale

7 ReturnLimit() 
Get amount of limit for MintLimit function

8 TimeWhenLimitIncrease()
Return unix Date when Owner can call IMLimit()

9 pauseTokens()
Owner sale can pause Token only through contract sale

10 unpauseTokens()
Owner sale can unpause Token only through contract sale

11 finishMint()
Owner sale can finish mint forever

12 blockCallPauseTokens()
Owner can block call pauseTokens FOREVER

13 isblockCallPauseTokens()
view status about the possibility of calling pauseTokens()

# Install
1) clone repo
2) cd
3) npm i --only=dev

# Test

1) truffle migrate
2) truffle test

# Deploy
0) Set infura_apikey and metamask mnemonic in truffle.js
1) Remove bild folder (if it is created)
2) Reset Metamask account
3) truffle migrate compile-all --network YOUR NETWORK

