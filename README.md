# task6
stock_prices = list(map(int, input("Enter stock prices separated by space: ").split()))
if not stock_prices or len(stock_prices) < 2:
    print(0)
else:
    min_price = stock_prices[0]
    max_profit = 0

    for price in stock_prices:
        min_price = min(min_price, price)
        max_profit = max(max_profit, price - min_price)

    print(max_profit)
