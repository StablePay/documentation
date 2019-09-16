---
description: >-
  The objective of this page is to guide the user to configure the widget for
  accept donations with StablePay.
---

# Donations

1. Choose Donation to generate your Widget.

![](../.gitbook/assets/image%20%2835%29.png)

**Note:** Donations and payments directly from DAI to DAI are free of fees to receive, will only incur the gas costs of the transaction.. Any other token will be converted and a small fee will be charge before receiving the final amount. Read more here: [https://stablepay.io/faqs](https://stablepay.io/faqs).

2. Create your list of options for the client, to donate DAIs. The default amount is going to be the first in the list.

![](../.gitbook/assets/image%20%282%29.png)

3. Put the address of your Ethereum wallet to receive DAIs.

![](../.gitbook/assets/image%20%2811%29.png)

If you don't have a wallet, you can start with a MetaMask wallet, is easy and fast. To learn more about it:[https://metamask.io/](https://metamask.io/) 

4. If you want that your payments go to **Compound** activate "Supply to Compound".

![](../.gitbook/assets/image%20%2812%29.png)

To learn more about **Compound**, visit their website: [https://compound.finance/](https://compound.finance/).

5. Name of the owner of the Ethreum wallet\(optional\).

![](../.gitbook/assets/image%20%289%29.png)

6. After donating, the widget is going to redirect to your store, put the address here.

![](../.gitbook/assets/image%20%2828%29.png)

### Donations with HTML

7.The code in HTML is going to be generated and you ready to paste it on your page!.

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
                    callbackURL: 'https:/mystore.com',
                    theme: 'colored',
                },
                'stablepay-widget'
            );
        </script>
    </body>
</html>
```

8. The code has to create a button similar to the one below.

![](../.gitbook/assets/image%20%2822%29.png)

9. When the client 'click' the button, he going to see a widget like this. where he/she can choose the token, which they prefer to use for donating.

![](../.gitbook/assets/image%20%2815%29.png)

10. Wait for the transaction been done, and now your client can be redirected to your store.

![](../.gitbook/assets/image%20%2813%29.png)

### Donations with Link

11. The link is going to be generated and you ready to paste it on your page or Github!.

```text
<a href="https://stablepay.io/checkout?data=U2FsdGVkX19IkPP%2Bx25neFHS%2Bzn97z7UwRyB1XCdy9E3Kbp4TLHCfaExoprtlIZY1u%2BHHwhkJpr9EYCNUgGPWcmh4xl22S6iWrp%2FqFkU3ZiZM4WI3B%2BkLtbAYTwBi3e4EweDpUfK1UTBtJSc57S2i1uil7DoYHbr43H%2FRfQathKzcjYM70zwZpBl77WVo6M0KMXzI5GH8pbizG8XkjwT97KqwLl3yPwHy%2B0FqLu1VGcZkRkCi8%2FfM4bs%2F0hzAy%2FdRMH%2FMpTPpTxCBTszmHc1%2FynziTH5e3eIQqk%2BL9AQqkNB6c2YNcK7e09az5PgH01m5KJA6dLoOhGRrivf2XtUunhMYmioGIAY%2B6O8zRiXAIicw15RL9y8e%2F3ZIoVBtTD0cUWuvvizGcTY3FM9xWFn7PnMqqLkN2MhXd7FFeOm1zaqgiGvwtCay4KkUSV61ilE">
    <img src="https://stablepay.io/static/DonationsButtonBlueWhite.svg" >
</a>
```

12. You can use the link in your Github repository, pasting the link in the **README.md** repository**.**

![](../.gitbook/assets/image%20%2834%29.png)

![](../.gitbook/assets/image%20%2816%29.png)

13. Wait for the transaction been done, and now your client can be redirected to your Github.

![](../.gitbook/assets/image%20%2827%29.png)

