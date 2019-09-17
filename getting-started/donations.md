---
description: >-
  If you want to embed the StablePay widget for donations or payments in your
  github repo or website follow the steps below. No signup or email required to
  start using StablePay.
---

# Donations

Head over to our [Widget Generator](https://stablepay.io/widget/generator) and follow these steps:

1. Choose Donation to generate your Widget.

![](../.gitbook/assets/image%20%2835%29.png)

**Note:** Donations and payments directly from the same token \(e.g DAI to DAI\) are free of fees to receive, and sender will only incur the gas costs of the transaction like any normal ethereum transaction. In the case of a token conversion it will incur in a small platform fee that will be deducted from the final amount. Read more here for details: [https://stablepay.io/faqs](https://stablepay.io/faqs).

1. Create your list of amount options for the user to donate in DAIs. The default amount is going to be the first in the list.

![](../.gitbook/assets/image%20%282%29.png)

1. Put the address of your Ethereum wallet where you want to receive your tokens.

![](../.gitbook/assets/image%20%2811%29.png)

If you don't have a wallet, we suggest you start with a MetaMask wallet, is easy and fast. To learn more about it see:[https://metamask.io/](https://metamask.io/)

1. If you want your tokens to be deposited to **Compound** activate "Supply to Compound". Tokens will be supplied to Compound using your provided Wallet address where you can start earning interest on your DAI tokens. You have complete access to withdraw the tokens at any time with your wallet address.

![](../.gitbook/assets/image%20%2812%29.png)

To learn more about **Compound**, visit their website: [https://compound.finance/](https://compound.finance/)

1. Name of the owner of the Ethreum wallet\(optional\). 

![](../.gitbook/assets/image%20%289%29.png)

1. After confirming a transaction, the widget will redirect to your web site of choice, put the web site URL here.

![](../.gitbook/assets/image%20%2828%29.png)

## Donations in a website using HTML option

7.The code in HTML is going to be generated for you and you can paste it into your page!.

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
                    type: 'Donation',
                    source: {
                        name: 'JOHN DOE',
                        address: '0x05b54683C2C02aa690DF8b25B18Cd89C37a44f0C'
                    },
                    amount: {
                        total: 5,
                        options: [5,10,15,25,30]
                    },
                    callbackURL: 'https://mycontentsite.com/donate/success',
                    theme: 'colored',
                },
                'stablepay-widget'
            );
        </script>
    </body>
</html>
```

1. The code will create a button similar to the one below.

![](../.gitbook/assets/image%20%2822%29.png)

1. When the users 'click' the button, a widget like this will appear where they can choose the token they want to use for donating.

![](../.gitbook/assets/image%20%2815%29.png)

1. Wait for the transaction to be completed, and now the user can be redirected to your provided URL.

![](../.gitbook/assets/image%20%2813%29.png)

## Donations with Github

1. The link is going to be generated and you can copy and paste it on your Github Repository to accept tips and donations directly.

```text
<a href="https://stablepay.io/checkout?data=U2FsdGVkX19IkPP%2Bx25neFHS%2Bzn97z7UwRyB1XCdy9E3Kbp4TLHCfaExoprtlIZY1u%2BHHwhkJpr9EYCNUgGPWcmh4xl22S6iWrp%2FqFkU3ZiZM4WI3B%2BkLtbAYTwBi3e4EweDpUfK1UTBtJSc57S2i1uil7DoYHbr43H%2FRfQathKzcjYM70zwZpBl77WVo6M0KMXzI5GH8pbizG8XkjwT97KqwLl3yPwHy%2B0FqLu1VGcZkRkCi8%2FfM4bs%2F0hzAy%2FdRMH%2FMpTPpTxCBTszmHc1%2FynziTH5e3eIQqk%2BL9AQqkNB6c2YNcK7e09az5PgH01m5KJA6dLoOhGRrivf2XtUunhMYmioGIAY%2B6O8zRiXAIicw15RL9y8e%2F3ZIoVBtTD0cUWuvvizGcTY3FM9xWFn7PnMqqLkN2MhXd7FFeOm1zaqgiGvwtCay4KkUSV61ilE">
    <img src="https://stablepay.io/static/DonationsButtonBlueWhite.svg" >
</a>
```

1. You can use the link in your Github repository, pasting the link in a **README.md** file repository**.**

![](../.gitbook/assets/image%20%2834%29.png)

![](../.gitbook/assets/image%20%2816%29.png)

1. Wait for the transaction to be done, and now the user can be redirected to your Github page.

![](../.gitbook/assets/image%20%2827%29.png)

For more information, you can visit our page:[https://stablepay.io/](https://stablepay.io/)

