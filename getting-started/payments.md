---
description: >-
  The objective of this page is to guide the user to configure the widget for
  accept payments with StablePay.
---

# Payments

1. Choose Payment to generate your Widget.

![](../.gitbook/assets/image.png)

**Note:** Note: Donations and payments directly from DAI to DAI are free of fees to receive. Any other token will be converted and a small fee will be charge before receiving the final amount. Read more here: [https://stablepay.io/faqs](https://stablepay.io/faqs)

2. Put the address of your Ethereum wallet to receive DAIs.

![](../.gitbook/assets/image%20%2821%29.png)

If you don't have a wallet, you can start with a MetaMask wallet, is easy and fast. To learn more about it:[https://metamask.io/](https://metamask.io/) 

3. If you want that your payments go to **Compound** activate "Supply to Compound".

![](../.gitbook/assets/image%20%2830%29.png)

To learn more about **Compound**, visit their website: [https://compound.finance/](https://compound.finance/).

4. Name of the owner of the Ethreum wallet\(optional\).

![](../.gitbook/assets/image%20%2816%29.png)

5. After the payment, the widget is going to redirect to your store, put the address here.

![](../.gitbook/assets/image%20%281%29.png)

6.The code is going to be generated and you ready to paste it on your page!.

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

**Important:** The variable 'amount', it has to be given by your page. This is the amount of the product or products, that the client wants to pay.

7. The code has to create a button similar to the one below.

![](../.gitbook/assets/image%20%2831%29.png)

8. When the client 'click' the button, he going to see a widget like this. where he/she can choose the token, which they prefer to use for payment.

![](../.gitbook/assets/image%20%2823%29.png)

9. Wait for the transaction been done, and now your client can be redirected to your store.

![](../.gitbook/assets/image%20%2827%29.png)

