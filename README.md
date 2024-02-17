def getdatapoint(stock_name, bid_price, ask_price):
"""
return a tuple of stock name, bid price, ask price and average price.
"""
average_price = (bid_price + ask_price) / 2
return stock_name
