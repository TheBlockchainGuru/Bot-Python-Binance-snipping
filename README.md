# binance-trading-bot-new-coins
This Binance trading bot detects new coins as soon as they are listed on the Binance exchange and automatically places sell and buy orders. 
It comes with trailing stop loss and other features.

This open source crypto trading bot should able able to quickly detect new coins listings on Binance and quickly ride the price spike. 
It comes with a live and test mode so naturally, use at your own risk.

## input account information

in auth/auth.yml

...
	  binance_api: "BINANCE_API_KEY"
 	  binance_secret: "BINANCE_SECRET"
      binance_tld: "BINANCE_TLD"
...


## input trade config variables.
in config.yml 

---
	  TRADE_OPTIONS:
	    # In your pairing coin
	    QUANTITY: 15
	    # BTCUSDT will be bought for example
	    PAIRING: USDT
	    # How often to check for posts and run the script
	    # in minutes
	    RUN_EVERY: 0.025
	    TEST: True
	    SL: 3
	    TP: 2
	    ENABLE_TSL: True
	    TSL: 4
	    TTP: 2
	  SEND_NOTIFICATIONS: True
	  EMAIL_ADDRESS: 'your@email.address'
	  EMAIL_PASSWORD: 'I'll let you figure out what this one is'


