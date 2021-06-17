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
