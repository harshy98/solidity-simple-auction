## solidity-simple-auction

### Features:
  * to submit bid
  * to withdraw bid when someone bids higher
  * to end auction and finally send eth to beneficiary after all bids are submitted 
### How it works:
  * enter a bid amount in makebid function **within** the bidding period
  * try changing sender's address to make a new bid OR bid with the same address, cases will be handled accordingly
  * you can also view who is the highest bidder and how much any address has bid
  * finally, to end the auction just set the highest bidder's address with the amount of eth staked by that address to be sent to beneficiary and call the endAuction() function
  * after ending auction, check if the highest bidder  is credited with the token or not by calling getHighestBidderBal()
### Note: before running script, change the startTime and endTime values in the constructor according to epoch time (get it at: https://www.epochconverter.com/) and then compile and deploy it. Also, set the beneficiary address before depoying in the "deploy and run transactions" plugin. Now, call using any other address to submit a bid.
