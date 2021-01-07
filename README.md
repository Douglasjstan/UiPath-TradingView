# UiPath-TradingView

This is binary option trading bot developed using UiPath to webscrap TradingView Technical Analysis site.  Based on the recommendation by TradingView, the bot will automatically open a CALL or PUT trade in Ayrex.com Broker.

Only AUDUSD and EURUSD pair are used because the payout in Ayrex.com for other currency pair is low.  To add new currency pair, new xaml has to be created.

Criteria:

For Call : Strength = "Strong Buy" And Buy > 18 And Sell < 2 And Neutral < 10
For Put  : Strength = "Strong Sell" And Sell > 18 And pBuy < 2 And Neutral < 10
