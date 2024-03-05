# Profitable Jetton

Mint of 100 total_coins from Jetton Minter to Jetton Wallets

> JW A coin_balance = 20
> JW B coin_balance = 40
> JW C coin_balance = 40 (DEX)

1000 TON come to Jetton Minter from Routing Pool

> Add 0:1000 TON to dividend_income_dict
> Jetton Minter Balance = 1000 TON

JW A sends msg with current_coins_amount to JM to get dividend income

> 1000 TON / 100 total_coins * 20 current_coins_amount = 200 TON comes to JW A
> JW A repaid_profit_dict: 0:200
> Jetton Minter Balance = 800 TON

2000 TON come to Jetton Minter from Routing Pool

> Add 2:2000 TON to dividend_income_dict
> profits_dict: 0:1000, 1:2000
> Jetton Minter Balance = 2800 TON

JW A sends msg with current_coins_amount to JM to get dividend income:

> (1000 TON + 2000 TON) / 100 total_coins * 40 current_coins_amount = 1200 TON to JW B
> JW B repaid_profit_dict: 0:400, 1:800
> Jetton Minter Balance = 1600 TON

JW A sells 10 coins to JW B

> JW A transfers 10 coins to JW C
> JW A Coin Balance = 10
> JW A repaid_profit_dict: 0:100
> JW C Coin Balance = 10
> JW C repaid_profit_dict: 0:100
> JW B sends payment for coin to JW C
> JW C transfers 10 coins to JW B
> JW C Coin Balance = 0
> JW C repaid_profit_dict: 0:0
> JW B Coin Balance = 50
> JW B repaid_profit_dict: 0:500, 1:800
