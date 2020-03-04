---
description: >-
  If you want to embed the StablePay widget for payments in your ecommerce
  website follow the steps below. No signup or email required to start using
  StablePay.
---

# Payments

1. Choose Payment to generate your Widget.

![](../.gitbook/assets/image.png)

**Note:** Donations and payments directly from the same token \(e.g DAI to DAI\) are free of fees to receive, and sender will only incur the gas costs of the transaction like any normal ethereum transaction. In the case of a token conversion it will incur in a small platform fee that will be deducted from the final amount. Read more here for details: [https://stablepay.io/faqs](https://stablepay.io/faqs).

1. Put the address of your Ethereum wallet where you want to receive your tokens.

![](../.gitbook/assets/image%20%2823%29.png)

If you don't have a wallet, we suggest you start with a MetaMask wallet, is easy and fast. To learn more about it see:[https://metamask.io/](https://metamask.io/)

1. If you want your tokens to be deposited to **Compound** activate "Supply to Compound". Tokens will be supplied to Compound using your provided Wallet address where you can start earning interest on your DAI tokens. You have complete access to withdraw the tokens at any time with your wallet address.

![](../.gitbook/assets/image%20%2832%29.png)

To learn more about **Compound**, visit: [https://compound.finance/](https://compound.finance/)

1. Name of the owner of the Ethreum wallet\(optional\).

![](../.gitbook/assets/image%20%2818%29.png)

1. After the payment, the widget is going to redirect to your website or store, put the website URL.

![](../.gitbook/assets/image%20%281%29.png)

1. The code is going to be generated and you ready to paste it on your page!.

```text
<!DOCTYPE html>
<html>
    <head>
        <!-- Add this <script> to the <head> tag -->
        <script src="https://unpkg.com/@stablepay/widget"></script>
    </head>
    <body>
        <!-- Add this anywhere in your site where you would like to render the Widget -->
        <div id="stablepay-widget"></div>

        <!-- Add this <script> at the end of the <body> tag -->
        <script>
            StablePay.renderWidgetButton(
                {
                    type: 'Payment',
                    source: {
                        name: 'John Doe',
                        address: '0x05b54683C2C02aa690DF8b25B18Cd89C37a44f0C'
                    },
                    amount: {
                        total: INSERT_AMOUNT_VARIABLE_HERE
                    },
                    callbackURL: 'https:/mystore.com',
                    postAction: {
                        action: 'compound'
                    },
                    theme: 'standard',
                },
                'stablepay-widget'
            );
        </script>
    </body>
</html>
```

**Important:** The variable 'amount' has to be provided by your page. This is the amount of the product or products, that the client wants to pay in your checkout page.

1. The code has to create a button similar to the one below.

![](../.gitbook/assets/image%20%2833%29.png)

1. When the users 'click' the button, they will see a widget similar to this. They can choose the token, which they prefer to use for payment.

![](../.gitbook/assets/image%20%2825%29.png)

1. Wait for the transaction to be done, and now the user can be redirected to your configured URL.

![](../.gitbook/assets/image%20%2829%29.png)

For more information, visit:[https://stablepay.io/](https://stablepay.io/)

