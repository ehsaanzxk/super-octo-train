def getDataPoint(stock_name, bid_price, ask_price):
    """
    Returns a tuple of stock name, bid price, ask price, and average price.
    """
    average_price = (bid_price + ask_price) / 2
    return stock_name, bid_price, ask_price, average_price

def getRatio(stock_a, stock_b):
    """
    Returns the ratio of the prices of stock A to stock B.
    """
    ratio = stock_a[3] / stock_b[3]  # price is at index 3 in the tuple
    return ratio

def main():
    # Sample data for stock A and stock B
    stock_A = getDataPoint("Stock A", 100, 105)
    stock_B = getDataPoint("Stock B", 95, 98)

    # Output stock info, prices, and ratio
    print("Stock A Info:")
    print("Name:", stock_A[0])
    print("Bid Price:", stock_A[1])
    print("Ask Price:", stock_A[2])
    print("Average Price:", stock_A[3])

    print("\nStock B Info:")
    print("Name:", stock_B[0])
    print("Bid Price:", stock_B[1])
    print("Ask Price:", stock_B[2])
    print("Average Price:", stock_B[3])

    ratio = getRatio(stock_A, stock_B)
    print("\nRatio of Stock A to Stock B Prices:", ratio)

# Entry point of the program
if __name__ == "__main__":
    main()
